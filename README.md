# Neural-Networks-on-Fashion-MNIST
Created a model to run on the Fashion MNIST data set to achieve the highest accuracy keeping in mind the feasibility and computational power. 16 models were created to study from to create a report which highlights which loss functions and activation functions lead to the highest accuracy keeping in mind run times.

For every model :-

● L2 regularization of 0.01 for every hidden layer

● Dropout of 0.20 has been used after the last hidden layer

● Learning rate = 0.0005

● Batch size = 32

● Epochs = 30

![image](https://user-images.githubusercontent.com/86141988/163631426-ea533e20-32a7-4802-ac41-cb9bcc772fd9.png)

● The general trend that we can observe here is that sigmoid activation
function works best followed by ReLU and then Tanh

● We can also say that increasing the number of hidden layers may not
necessarily lead to better results (this is evident from how for a particular
set of activation and loss function, increasing number of layer does not
improve accuracy - Eg: Models 6&7, Models 14&15, Models 11&12 but
increases accuracy in a few other instances - Eg: Models 12&13,)

○ Increasing the number of layers helps us learn more complex
features, thus always increasing the training accuracy

○ Sometimes due to overfitting,i.e, due to the larger number of
parameters, model fits too closely to the training data, thus losing its
ability to generalize well and performing badly on the validation set
(evident by lower validation accuracy in spite of higher training
accuracy)

● Increasing the number of neurons in a hidden layer can lead to better
results and can have a greater effect than changing activation function
(evident from comparing Models 3&4 - Model 4 performed better even
though in Model 3 sigmoid activation function has been used)

○ By increasing the number of neurons, we are able to learn more
complex features. However activation functions only introduces
non-linearity into the output and the choice of the activation function
does not make a huge impact

● Another inference we can make is that KL divergence works better than
Categorical Cross Entropy (Can be inferred by comparing Models 2&3)

● Increasing the number of hidden layers comprises the computational
feasibility causing high runtimes. (We can see from Models 8&16 that this
holds true.)
