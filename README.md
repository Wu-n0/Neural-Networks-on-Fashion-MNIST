# Neural-Networks-on-Fashion-MNIST

This project focuses on creating a model to achieve the highest accuracy on the Fashion MNIST dataset while considering feasibility and computational power. Sixteen models were created and analyzed to identify the optimal combination of loss functions and activation functions that result in the highest accuracy within reasonable run times.

## Dataset and Model Architecture

The Fashion MNIST dataset was used for training and evaluation. The models were designed with various configurations to study the impact of different loss functions and activation functions on accuracy. L2 regularization with a value of 0.01 was applied to every hidden layer, and a dropout of 0.20 was implemented after the last hidden layer.

## Training Parameters

During training, the following parameters were used consistently across the models:

- Learning rate: 0.0005
- Batch size: 32
- Epochs: 30

These parameters were chosen to strike a balance between achieving accurate results and optimizing computational efficiency.

## Model Analysis

The analysis of the sixteen models revealed interesting insights:

- Sigmoid activation function consistently yielded the highest accuracy, followed by ReLU and then Tanh.
- Increasing the number of hidden layers did not always lead to improved accuracy. In some cases, increasing the number of layers did not significantly impact accuracy, while in other cases, it led to overfitting and decreased validation accuracy.
- Increasing the number of neurons in a hidden layer had a greater impact on results compared to changing the activation function. Increasing the number of neurons allowed the model to learn more complex features.
- KL divergence outperformed Categorical Cross Entropy as the chosen loss function in terms of accuracy.

![Model Comparison](https://user-images.githubusercontent.com/86141988/163631426-ea533e20-32a7-4802-ac41-cb9bcc772fd9.png)

## Results and Conclusions

The analysis of the models highlighted the importance of selecting appropriate activation functions, optimizing the number of hidden layers, and considering the impact of loss functions on accuracy. The findings can serve as a guide for designing neural networks for similar tasks and datasets.

Feel free to explore the source code and experiment with different configurations. Further details and insights can be found in the project report.
