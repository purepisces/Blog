# Neural Networks Overview


We will learn about what neural networks do and how they do it.
For example, different dosages will have different efficacy, and we can not just fit a line for the dataset. But even if we have a really complicated dataset like this, a neural network can fit a squiggle to it.

<img src="nn_squiggle.png" alt="nn_squiggle" width="400" height="300"/>

## What is a Neural Network?

A neural network is composed of layers of nodes, with connections between these nodes. The values along each connection represent the parameters of the network, which are estimated during the training process.

<img src="connection_value.png" alt="connection_value" width="400" height="300"/>

For now, just know that these parameter estimates are analogous to the slope and intercept values that we solve for when we fit a straight line to data. 

Initially, the parameter values of a neural network are unknown. These values are determined through a process called backpropagation, which adjusts the parameters to fit the network to the training data.


<img src="unknown_value.png" alt="unknown_value" width="400" height="300"/> <img src="back_estimated.png" alt="back_estimated" width="400" height="300"/>

And we will talk about how backprogagation estimates these parameters in part2 in this series, but for now, just assume that we’ve already fit this neural network to this specific dataset and that means we have already estimated these parameters. 

### Activation Function

Also, you may have noticed that some of the nodes have curved lines inside of them, the curved or bent lines are called activation functions. When you build a neural network, you have to decide which activation function or functions you want to use.

<img src="curved_lines.png" alt="curved_lines" width="400" height="300"/>

### Hidden Layers

The layers between the input and output layers are known as hidden layers. The configuration of these layers—how many there are and how many nodes they contain—is one of the initial design decisions when constructing a neural network.

<img src="hidden_layers.png" alt="hidden_layers" width="400" height="300"/>

### Constructing the Model

Let’s learn how this neural network creates new shapes from the curved or bent lines in the hidden layer and then adds them together to get a green squiggle that fits the data. Note in this neural network, we have one input node which is dosage, one hidden layer with 2 nodes and one output node which is efficacy.


<img src="add_together.png" alt="add_together" width="400" height="300"/>

#### Example: Dosage and Efficacy

Consider a scenario where we model the efficacy of a drug based on its dosage, ranging from 0 (low) to 1 (high). The neural network takes the dosage value, applies transformations through the network's parameters and activation functions, and outputs an efficacy prediction.

Note: To keep the math simple, let’s assume dosages go from 0(low) to 1(high).

The first thing we are going to do is plug the lowest dosage 0 into the neural network. Now, to get from the input node to the top node in the hidden layer, this connection multiplies the dosage by -34.4 and then adds 2.14 and the result is an x-axis coordinate for the activation function.

<img src="from_to.png" alt="from_to" width="400" height="300"/>

$(\text{Dosage} \times -34.4) + 2.14 = \text{x-axis coordinate}$

$(0 \times -34.4) +2.14 = 2.14$

<img src="x_axis_coordinate.png" alt="x_axis_coordinate" width="400" height="300"/>

To get the corresponding y-axis value, we plug 2.14 into the activation function, which, in this case, is the softplus function. Then we put a blue dot at 2.25 for dosage = 0.

<img src="choose_softplus.png" alt="choose_softplus" width="400" height="300"/> <img src="put_dot.png" alt="put_dot" width="400" height="300"/>

Note, if we had chosen the sigmoid curve for the activation function, then we would plug 2.14 into the equation for the sigmoid curve.

<img src="choose_sigmoid.png" alt="choose_sigmoid" width="400" height="300"/>

And if we continue to increase the dosage values all the way to 1(the maximum dosage), we get this blue curve.

<img src="blue_curve.png" alt="blue_curve" width="400" height="300"/>

Note, the full range of dosage values, from 0 to 1 corresponds to this relatively narrow range of values from the activation function. When we plug dosage values, from 0 to 1 into the neural network, and then multiply them by -34.4 and add 2.14, we only get x-axis coordinates that are within the red box and thus, only the corresponding y-axis values in the red box are used to make this new blue curve.

<img src="narrow_range.png" alt="narrow_range" width="400" height="300"/>

Now we scale the y-axis values for the blue curve by -1.30. For example, when dosage = 0, the current y-axis coordinate for the blue curve is 2.25, then 2.25*-1.3 = -2.93 which corresponds to this position on the y-axis. And we end up with a new blue curve.

<img src="scale_pos.png" alt="scale_pos" width="400" height="300"/> <img src="new_blue_curve.png" alt="new_blue_curve" width="400" height="300"/>

Now let’s focus on the connection from the input node to the bottom node in the hidden layer. Remember, for -2.52 and 1.29, these values come from fitting the neural network to the data with back propagation, and we’ll talk about that in part2 in this series.

<img src="remember.png" alt="remember" width="400" height="300"/>

Then same operation as before, we get this orange curve.

<img src="orange_curve.png" alt="orange_curve" width="400" height="300"/>


So we see that fitting a neural network to data gives us different parameter estimates on the connections and results in each node in the hidden layer using different portions of the activation functions to create these new and exciting shapes.

<img src="diff_para.png" alt="diff_para" width="400" height="300"/> <img src="diff_portion.png" alt="diff_portion" width="400" height="300"/> <img src="exciting_shape.png" alt="exciting_shape" width="400" height="300"/>


Now just like before, we scale the y-axis coordinates on the orange curve. Only this time, we scale by a positive number 2.28, and that gives us this new orange curve.

<img src="new_orange_curve.png" alt="new_orange_curve" width="400" height="300"/>


Now the neural network tells us to add the y-axis coordinates from blue curve to the orange curve, and that gives us this green squiggle.


<img src="add_curve.png" alt="add_curve" width="400" height="300"/>


Then finally we subtract 0.58 from the y-axis values on the green squiggle and we have a green squiggle that fits the data.

<img src="subtract_curve.png" alt="subtract_curve" width="400" height="300"/>

### Predictions

Now if someone comes along and says that they are using dosage = 0.5 we can look at the corresponding y-axis coordinate on the green squiggle and see that the dosage will be effective or we can solve for the y-axis coordinate by plugging dosage = 0.5 into the neural network and do the math. And we see that the y-axis coordinate on the green squiggle is 1.03, and since 1.03 is closer to 1 than 0, we will conclude that a dosage = 0.5 is effective.

<img src="BFSFMs.png" alt="BFSFMs" width="400" height="300"/>

### Weights and Biases

The parameters that we multiply are called weights and the parameters that we add are called biases.

<img src="weights.png" alt="weights" width="400" height="300"/> <img src="biases.png" alt="biases" width="400" height="300"/>

Note, this neural network starts with two identical activation functions, but the weights and biases on the connections slice them, flip them and stretch them into new shapes, which are then added together to get a squiggle that is entirely new, and the squiggle is then shifted to fit the data.

<img src="shift_data.png" alt="shift_data" width="400" height="300"/>

In theory, neural networks can fit a green squiggle to just about any dataset, no matter how complicated!

<img src="theory_nn.png" alt="theory_nn" width="400" height="300"/>

## Reference:
- [Watch the video on YouTube](https://www.youtube.com/watch?v=CqOfi41LfDw)