$1^T$ is a common notation in linear algebra that denotes a row vector where all the elements are ones.

---------------------------------

A **unit basis** (also known as a standard basis vector or elementary vector) is a vector in which one element is 1 and all other elements are 0. 

#### Definition
For a vector space $\mathbb{R}^k$, the unit basis vectors are denoted as $e_i$, where $i$ is the position of the 1 in the vector. Each unit basis vector has the following properties:

$$e_i = [0, 0, \ldots, 1, \ldots, 0]$$

Here, the \(i\)-th position is 1, and all other positions are 0.

#### Examples
**For $\mathbb{R}^3$**:

$$e_1 = [1, 0, 0]$$

$$e_2 = [0, 1, 0]$$

$$e_3 = [0, 0, 1]$$

#### Usage in Machine Learning
**One-Hot Encoding**:

In classification tasks, categorical variables are often converted into one-hot encoded vectors. For instance, if you have three classes (A, B, and C), you can represent class A as $e_1 = [1, 0, 0]$, class B as $e_2 = [0, 1, 0]$, and class C as $e_3 = [0, 0, 1]$.