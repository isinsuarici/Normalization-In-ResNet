# Residual Network (ResNet) with Different Normalization Techniques
This project implements a Residual Network (ResNet) model using PyTorch for image classification on the CIFAR-10 dataset. The ResNet architecture is enhanced with various normalization techniques to compare their effects on model performance.

<h2>Project Structure</h2>
The project consists of the following components:

<h4>1. Data Loading and Preprocessing (data_loader function):</h4>

The data_loader function loads and preprocesses the CIFAR-10 dataset. It applies transformations such as resizing, converting to tensors, and normalization. The function supports loading both training and validation data as well as the test data.

<h4>2. Normalization Layer Selection (get_normalization_layer function):</h4>

This function provides a selection of different normalization layers: Batch Normalization, Group Normalization, Instance Normalization, and Layer Normalization. The selected normalization technique is used in the convolutional layers of the ResNet.

<h4>3. Residual Block Implementation (ResidualBlock class):</h4>

The ResidualBlock class defines a single residual block used within the ResNet architecture. Each block contains two convolutional layers with the chosen normalization technique and a residual connection. The downsample option is used for downsampling the input when needed.

<h4>4. Residual Network Implementation (ResNet class):</h4>

The ResNet class constructs the ResNet architecture with multiple layers of residual blocks. The architecture includes initial convolutional layers, max-pooling, and several layers of residual blocks with varying numbers of channels and layers. The final classification is performed using an average pooling layer followed by a fully connected layer.

<h4>5. Model Training and Evaluation:</h4>

The script includes a training loop that iterates over different normalization techniques. For each technique, the model is trained on the training dataset and evaluated on the validation dataset. The training progress, loss, and validation accuracy are displayed.

<h4>6. Accuracy Comparison Plotting:</h4>

After training with different normalization techniques, the project generates a bar plot to compare the accuracies achieved by each technique on the validation dataset.

<h2>Results</h2>
The code demonstrates the impact of different normalization techniques on the ResNet model's performance. After training for a certain number of epochs, the script presents the accuracy achieved by each technique on the validation dataset. The final plot visually compares the accuracy achieved by each normalization technique.
<p>

![download](https://github.com/isinsuarici/Normalization-In-Resnet/assets/44557162/b9357c25-3ba1-4fa9-b48f-d726103912a3)
