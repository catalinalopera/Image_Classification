# AlexNet Architecture
# Why?
-> It Is a type of convolutional neural network (CNN) which is particularly suited for image
processing.<br></br>
-> This model effectively captures the spatial features that are critical for recognizing emotions on
faces.<br></br>
# How?
We trained two different models to see how they Learn Over Time.<br></br>
Model 1: Emotion Detection using basic Alexnet Architecture.<br></br>
Model 2: Emotion Detection using Alexnet Architecture + Data Augmentation + BatchNormalization.<br></br>
# AlexNet Observations:
-> Model 2 incorporates batch normalization layers, which significantly improve its training and
validation accuracies compared to Model 1. This suggests that batch normalization helps in
stabilizing the learning process by normalizing the input layer by adjusting and scaling the
activations. <br></br>
-> Enhancements for Model 2: Although Model 2 performs significantly better, we consider further
tuning. This could include adjusting the learning rate, experimenting with different optimizers, or
implementing more sophisticated data augmentation techniques. Additionally, exploring other
regularization techniques or modifying the architecture could yield better results.<br></br>
-> Regularization and Hyperparameter Optimization: For both models, we consider as an option
using regularization techniques such as L1/L2 regularization in the dense layers and conduct
thorough hyperparameter optimization to find the best settings for parameters such as the
learning rate, batch size, and the number of epochs.<br></br>
-> Cross-Validation: We conclude in the future the possibility to implement k-fold cross-validation to
ensure that the model's performance is consistent across different subsets of the data, providing
a more reliable estimate of its ability to generalize.<br></br>

# VGG16 Architecture
# Why?
-> VGG16 has been pre-trained on a vast dataset of images, making it capable of leveraging
transfer learning to significantly reduce the time and data needed to train an effective emotion
detection model.<br></br>
-> The architecture uses a series of convolutional layers with small filters followed by max-pooling
layers, allowing it to efficiently learn features at various levels of abstraction.
# How?
We trained three different models to see how they Learn Over Time.<br></br>
Model 1: Emotion Detection using basic VGG16 Architecture.<br></br>
Model 2: Emotion Detection using VGG16 Architecture and fine tuning, freezing layers.<br></br>
Model 3: Emotion Detection using VGG16 Architecture and fine tuning, freezing layers, including
dropout for regularization.<br></br>
# VGG16 Observations:
-> Model 3 takes a closer look at how well it can learn by only allowing changes to the last four
layers of VGG16. It also uses dropout to avoid overfitting, which is a smart way to make use of
deep learning features that have already been learned. At the same time, it fine-tunes the end
of the model to make it work better for the specific job it's meant to do. <br></br>
-> Data Augmentation: We conclude that increasing the variety and volume of training data
through more aggressive data augmentation could help the models generalize better to unseen
data. <br></br>
-> Regularization Techniques: We agree on experimenting with different regularization techniques,
such as L1/L2 regularization or varying the dropout rates, could provide a better balance
between learning and overfitting. <br></br>
-> Model Complexity: We agree in adjusting the model complexity by experimenting with the
number of layers and neurons in the custom layers added to the VGG16 base might help find a
sweet spot that minimizes overfitting while maintaining high performance.<br></br>
-> Learning Rate Adjustments: Also, we conclude that implementing learning rate schedules or
finding an optimal learning rate could improve training effectiveness and potentially enhance
validation performance.
