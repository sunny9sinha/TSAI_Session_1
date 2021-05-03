# TSAI_Session_1
Session_1 Assignment

What is a neural network neuron?
- A Neural network neuron is a mathematical unit or building block of a neural network. It has summation and an activation function as its component.
- These functions operate on the incoming signals from previous layer neurons or input.
- The summation happens after multiplying the incoming signals with its weight.

What is the use of the learning rate?
- It is a configurable hyperparameter in a neural network.
- This is the rate at which neural network adapts to the given problem.
- It ranges between 0 to 1 and, it has following effect.
- smaller the learning rate , more time it takes for the network to reach the minimum or converge.
- If this is large enough then it causes drastic updates and leads to divergent behavior.
- If this is just right then it reaches the minimum point swiftly.
- From the equation :
-                    ![image](https://user-images.githubusercontent.com/83466398/116865709-c7c1c900-ac27-11eb-80e8-309c3cdde2f4.png)
                     We can see how LR (Learning Rate) affects the new weight calculation during backpropagation, it controls the rate at which the weight of a signal changes and reaches optimum value to reduce the error.
                     
How are weights initialized?
- Weights are initialized using following strategies :
          - Xavier initialization : This approach sets a layer's weight randomly from a uniform distribution bound between
                                    ±sqrt(6)/sqrt(ni + ni+1) , where ni is the number of incoming network connections to the layer and ni+1 is the number of outgoing                                         network connections from the layer. 
          - Kaiming initialization : This is mainly for neural networks with RELU like activation functions.In this approach we populate weight with numbers randomly                                         chosen from a standard normal distribution. Then multiply these numbers with sqrt(2)/sqrt(n), where n is the number of incoming                                           signals or connections from previous layer to given layer. Then we initialize bias to be zero.

What is "loss" in a neural network?
- Loss in a neural network is the error in prediction. It is the difference in desired value and the obtained value.

What is the "chain rule" in gradient flow?
- It is the partial derivative rule to calculate the derivative of a function which is a combination of other functioins.
- For example, if we have a function Z = h(X,Y) where X = f(t) and Y = g(t) then derivative of Z with respect to t will be calulated as :
-     del(Z)/del(t) = (del(Z)/del(X))(del(X)/del(t)) + (del(Z)/del(Y))(del(Y)/del(t))  
