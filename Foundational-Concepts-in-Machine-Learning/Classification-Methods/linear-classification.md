# Linear Classification

Previously, we explored Image Classification, which involves assigning a single label to an image from a predefined category set. We discussed the k-Nearest Neighbor (kNN) classifier, which labels images by comparing them to labeled examples in the training set. However, kNN has some drawbacks:

-   The classifier needs to retain all training data to compare against new test data, which can be inefficient in terms of storage because datasets may easily be gigabytes in size.
-   Classifying a new image is computationally expensive, as it demands comparisons with each training image.

### Overview

Now, we’ll develop a more robust approach to image classification, eventually extending to Neural Networks and Convolutional Neural Networks (CNNs). This approach has two key elements: a **score function** that maps raw data to class scores, and a **loss function** that quantifies the agreement between predicted scores and actual labels. By minimizing the loss function with respect to the score function’s parameters, we can optimize the model.

### Parameterized mapping from images to label scores

The first step is defining a score function that maps the pixel values of an image to confidence scores for each class. Let’s walk through this with an example. Suppose we have a training dataset of images $x_i \in R^D$ paired with labels $y_i$, where $i = 1 \dots N$ and $y_i \in { 1 \dots K }$. Here, **N** represents the number of examples, **D** the dimensionality of each image, and **K** the number of categories. For instance, in CIFAR-10, there are **N** = 50,000 images, each with **D** = 32 x 32 x 3 = 3072 pixels, and **K** = 10 classes (e.g., dog, cat, car, etc). We now define the score function $f: R^D \mapsto R^K$, mapping raw image pixels to class scores.

#### Linear Classifier

 In this module we will start out with arguably the simplest possible function, a linear mapping:
 
$$f(x_i, W, b) = W x_i + b$$

In this equation, we assume that the image $x_i$ is represented as a flattened column vector with a shape of $[D \times 1]$. The matrix $W$ has dimensions $[K \times D]$, and the vector $b$ has dimensions $[K \times 1]$; together, they are the parameters of this function. For CIFAR-10, each image $x_i$​ is flattened into a column vector of shape $[3072 \times 1]$, so $W$ is $[10 \times 3072]$, and $b$ is $[10 \times 1]$. As a result, 3072 values (the raw pixel values) are input into the function, producing 10 values as outputs (the class scores). The entries in $W$ are commonly referred to as weights, while $b$ is known as the bias vector, which adjusts the output scores independently of the data in $x_i$. However, it is common for weights and parameters to be used interchangeably.

Key points:

-   Each row of **W** acts as a separate classifier, so **W** effectively evaluates multiple classifiers simultaneously. For example, if we have three classes—**ship**, **cat**, and **dog**—then row 1 in the weight matrix would contain the weights for the "ship" classifier, row 2 for the "cat" classifier, and row 3 for the "dog" classifier.
-   Our objective is to adjust **W** and **b** such that scores align with ground truth labels across the dataset.
-   A major advantage: once the parameters **W** and **b** are learned, the training set isn’t needed for classification, as new images are classified using the learned parameters alone.
-   Finally, it's worth noting that classifying a test image only requires a single matrix multiplication and addition, making it much faster than comparing the test image to every training image.

> **Foreshadowing**: CNNs will build on this framework, mapping image pixels to scores with more complex functions and parameters.

### Interpreting a linear classifier

A linear classifier determines the score for each class by calculating a weighted sum of pixel values across all three color channels in an image. The classifier’s function can assign positive or negative significance to specific colors in certain areas based on the values of these weights. For example, for a "ship" class, a strong presence of blue pixels along the edges of an image might indicate water. In this case, the classifier could have positive weights in the blue channel (indicating that more blue boosts the likelihood of a ship) and negative weights in the red and green channels (indicating that red or green decreases the likelihood of a ship).
___
insert img

This example illustrates how an image is mapped to class scores. For simplicity, we consider an image composed of just 4 monochrome pixels, and we have 3 classes represented as red (cat), green (dog), and blue (ship). Please note that the colors here denote the classes and are not related to RGB channels. We will flatten the image pixels into a column vector and perform matrix multiplication to calculate the scores for each class. It's important to point out that this specific weight matrix $W$ is not effective, as it assigns a very low score to the cat class despite the image being of a cat. In fact, this weight configuration suggests that the model is more inclined to classify it as a dog.
___


**Analogy of Images as High-Dimensional Points**

Since images can be represented as high-dimensional column vectors, we can think of each image as a point in a high-dimensional space. For example, in the CIFAR-10 dataset, each image is represented as a point in a 3072-dimensional space, corresponding to the 32x32x3 pixel dimensions. Consequently, the entire dataset can be viewed as a labeled set of these points.

We defined the score of each class as a weighted sum of all image pixels, which means that each class score is a linear function over this space. Although we can't visualize a 3072-dimensional space, we can imagine compressing all these dimensions into two for visualization purposes. This allows us to conceptualize how the classifier operates.

insert img

A cartoon representation of image space, illustrating that each image is a point, and three classifiers are visualized. For instance, the red line for the car classifier indicates all points that receive a score of zero for the car class. The red arrow shows the direction of increasing scores, meaning all points to the right of the line have positive and linearly increasing scores, while those to the left have negative and linearly decreasing scores.
___

As previously mentioned, each row of the weight matrix $W$ represents a classifier for one of the classes. Geometrically, modifying a row in $W$ alters the corresponding line in pixel space, causing it to rotate in different directions. The bias terms $b$ allow our classifiers to translate these lines. Notably, without bias terms, if we plug in $x_i = 0$, the score will always be zero, regardless of the weights, forcing all lines to intersect at the origin.

**Interpretation of linear classifiers as template matching.** Another way to interpret the weights $W$ is to view each row as a _template_ (or _prototype_) for a class. The score for each class is then derived by comparing the corresponding template with the image using an _inner product_ (or _dot product_). In this context, the linear classifier performs template matching, with the templates learned from the data. This approach can be thought of as a variant of the Nearest Neighbor method, where instead of utilizing numerous training images, we rely on a single template per class (which is learned rather than drawn from the training set). In this case, the (negative) inner product serves as the distance metric instead of traditional L1 or L2 distances.
___
insert img

Looking ahead: Example learned weights after training on CIFAR-10. For instance, the ship template prominently features blue pixels, indicating that this template will yield a high score when matched against images of ships in the ocean through the inner product. 
___

Additionally, it's noteworthy that the horse template appears to include features from both left- and right-facing horses due to the dataset's diversity. This results in the linear classifier merging these variations into a single template. Similarly, the car classifier seems to combine several variations into a single template that must identify cars from all angles and colors. In this case, the template appears predominantly red, suggesting that red cars are more prevalent in the CIFAR-10 dataset. The linear classifier's simplicity makes it challenging to effectively differentiate between colors, a limitation that will be addressed in neural networks. Neural networks can create intermediate neurons in hidden layers to detect specific car types (e.g., green cars facing left, blue cars facing front) and subsequently combine these detections into a more precise car score through weighted sums.

**The Bias Trick**

Before we proceed, it's useful to mention a common technique for simplifying the representation of the parameters $W$ and $b$. Recall that we defined the score function as:

$$f(x_i, W, b) = W x_i + b$$

As we delve deeper into the material, managing two sets of parameters (the weights $W$ and the biases $b$) can become cumbersome. A widely used method is to combine these parameters into a single matrix by adding an extra dimension to the vector $x_i$, which always holds the constant value $1$—this is known as the _bias dimension_. With this adjustment, the new score function simplifies to a single matrix multiplication:

$$f(x_i, W) = W x_i$$

In our CIFAR-10 example, $x_i$ now becomes a $3073 \times 1$ vector instead of $3072 \times 1$ (with the added dimension holding the constant $1$), and $W$ is now $10 \times 3073$ instead of $10 \times 3072$. The additional column in $W$ corresponds to the bias $b$. An illustration can help clarify this:

insert img

Illustration of the bias trick. Performing matrix multiplication and then adding a bias vector (left) is equivalent to adding a bias dimension with a constant value of 1 to all input vectors and extending the weight matrix by one column to include a bias column (right). By preprocessing our data to append ones to all vectors, we only need to learn a single weight matrix instead of managing two separate matrices for weights and biases. 

**Image Data Preprocessing**

As a brief note, in the examples above, we used raw pixel values that range from [0...255]. In machine learning, it is standard practice to normalize input features (with each pixel treated as a feature). Specifically, it is important to **center the data** by subtracting the mean from each feature. For images, this means calculating a _mean image_ across all training images and subtracting it from each image, resulting in pixel values ranging from approximately [-127 ... 127]. Another common preprocessing step is to scale each input feature so that its values fall within the range [-1, 1]. While zero-mean centering is arguably the more critical step, we will explore its significance further as we understand the dynamics of gradient descent.

### Loss function