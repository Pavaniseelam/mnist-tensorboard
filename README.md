Neural Network Experiments with TensorFlow

Student Details

Name: Pavani Seelam 

Student ID: 700756483

**Project Overview**

This project covers fundamental neural network operations, including tensor manipulations, loss function evaluations, model training with different optimizers, and logging results using TensorBoard. The tasks were implemented using TensorFlow and Keras.

**Tasks Completed**

**1. Tensor Manipulations & Reshaping**

Created a random tensor of shape (4,6).

Found its rank and shape using TensorFlow functions.

Reshaped the tensor into (2,3,4) and transposed it to (3,2,4).

Broadcasted a smaller tensor of shape (1,4) to match the larger tensor and performed element-wise addition.

Concept Explanation: Broadcasting allows TensorFlow to automatically expand smaller tensors to match the shape of larger tensors when performing operations.

**2. Loss Functions & Hyperparameter Tuning**

Defined true values (y_true) and model predictions (y_pred).

Computed Mean Squared Error (MSE) and Categorical Cross-Entropy (CCE) loss values.

Modified predictions slightly and observed changes in loss values.

Plotted a bar chart comparing MSE and Cross-Entropy loss using Matplotlib.

**3. Training a Model with Different Optimizers**

Loaded the MNIST dataset for digit classification.

Built and trained two neural network models:

One using Adam optimizer.

Another using SGD (Stochastic Gradient Descent) optimizer.

Compared training and validation accuracy for both models.

Observations: The Adam optimizer generally converges faster than SGD.

**4. Train a Neural Network and Log to TensorBoard**

Loaded and preprocessed the MNIST dataset.

Built a simple feedforward neural network.

Enabled TensorBoard logging and stored logs in the "logs/fit/" directory.

Launched TensorBoard to analyze loss and accuracy trends.

**4.1 Questions Answered**

Patterns in training & validation accuracy curves:

Accuracy generally increases over time, but validation accuracy may plateau or drop due to overfitting.

Detecting overfitting using TensorBoard:

If training loss keeps decreasing but validation loss increases, overfitting is occurring.

Effect of increasing epochs:

More epochs improve accuracy initially, but after a certain point, overfitting may occur.

How to Run the Project

Clone the repository:

git clone [your-github-repo-url]
cd [your-repo-folder]

**Install dependencies:**

pip install tensorflow matplotlib

Run the Tensor Manipulations script:

python tensor_manipulations.py

Run the Loss Function Comparison script:

python loss_functions.py

Train models with Adam and SGD optimizers:

python train_mnist.py

Run TensorBoard to analyze training logs:

tensorboard --logdir=logs/fit/

Then, open http://localhost:6006/ in your browser.
