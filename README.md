# Extreme Learning Machine & Multilayer Perceptron

* <h4><b> Overview </b></h4> 

  In this project, the performance of Extreme Learning Machines (ELM) and Multilayer Perceptrons (MLP) is compared for the task of handwritten digit recognition using the EMNIST dataset. The dataset is pre-processed, with images resized to a consistent shape and normalized to ensure proper model training. Both ELM and MLP models are implemented using Keras. The ELM model leverages a single hidden layer with random weights and a fast training process, while the MLP model consists of multiple layers with backpropagation for weight adjustment. The project involves training both models and evaluating their performance using accuracy metrics and loss curves. The results highlight the strengths and weaknesses of both models in terms of training speed, predictive accuracy, and suitability for digit classification tasks. The code also visualizes the loss and accuracy curves for both models, offering insights into their convergence and generalization capabilities.

* <h4><b> Key Findings </b></h4> 

  - <b> Training Efficiency: </b> The ELM model demonstrated faster training times due to its random weight assignment in the hidden layer, while the MLP model, with its multiple layers and backpropagation, took longer to train but showed more fine-tuned weight adjustments.
  - <b> Accuracy Performance: </b> Both models achieved high accuracy, but the MLP model slightly outperformed the ELM in terms of overall predictive accuracy, particularly when fine-tuning hyperparameters like the number of neurons and learning rate.
  - <b> Loss Convergence: </b> The MLP model exhibited a gradual decrease in loss over epochs, indicating stable convergence during training. In contrast, the ELM model's loss curve showed rapid convergence but also had more fluctuation, reflecting its reliance on random weight initialization.
  - <b> Generalization Capabilities: </b> The MLP's multi-layered architecture allowed it to generalize better on unseen test data, producing slightly lower test loss compared to the ELM model, which was more prone to overfitting with less structured training.
  - <b> Visualization of Performance: </b> The accuracy and loss curves for both models were plotted and compared, with the MLP model showing more consistent performance across epochs, while the ELM model's performance varied more with training iterations.

* <h4><b> Insightful Details </b></h4> 

  - <b> ELM’s Speed Advantage – </b> The Extreme Learning Machine (ELM) demonstrated a significant advantage in training speed due to its random initialization of weights in the hidden layer and one-pass learning process, making it ideal for large-scale problems where training time is critical.
  - <b> MLP’s Robustness with Hyperparameter Tuning – </b> The MLP model showed improved robustness as hyperparameters, such as the number of neurons and learning rate, were adjusted. This allowed the model to fine-tune its weights more precisely, enhancing its performance over time compared to the more rigid structure of the ELM.
  - <b> Accuracy Trade-Off – </b> While both models reached high accuracy, the MLP generally outperformed ELM on more complex datasets, demonstrating its ability to capture intricate patterns in the data through its deep architecture. However, ELM achieved comparable performance on simpler datasets.
  - <b> Loss Behavior and Overfitting – </b> The MLP showed smoother loss reduction over epochs, indicating that the model was gradually improving. The ELM, however, experienced more erratic loss fluctuations due to its random weight assignment, highlighting its potential sensitivity to overfitting when not properly tuned.
  - <b> Data Preprocessing Impact – </b> The success of both models in accurately predicting data was heavily influenced by preprocessing steps such as feature scaling. For both models, using the MinMaxScaler helped normalize the data, leading to more stable and predictable outcomes, particularly in the case of ELM’s reliance on scaled input data.

* <h4><b> Challenges </b></h4> 
 
  - <b> ELM Sensitivity to Data Variations – </b> The Extreme Learning Machine (ELM) model exhibited high sensitivity to variations in input data. Since the weights are initialized randomly, small changes in the data could significantly affect the model's performance, requiring careful preprocessing and feature scaling.
  - <b> Choosing Optimal Hyperparameters for MLP – </b> Finding the right number of neurons, layers, and learning rate for the MLP model proved to be a challenge. Inconsistent tuning of these hyperparameters led to variations in performance, with the model sometimes struggling to converge if the parameters were not carefully selected.
  - <b> Training Time for Complex Datasets – </b> While ELM offers fast training for simple problems, it struggled with larger and more complex datasets. On the other hand, MLP, though more accurate, required longer training times, especially when hyperparameters were not optimized, which added complexity to the project.
  - <b> Overfitting in MLP – </b> Despite tuning, the MLP model exhibited overfitting on smaller datasets, where the training accuracy was significantly higher than the testing accuracy. This highlighted the need for additional regularization techniques or a larger dataset to prevent overfitting.
  - <b> Model Generalization – </b> Both models faced challenges with generalization to unseen data. The ELM, due to its random initialization, required careful tuning to avoid underfitting or overfitting, while MLP needed strategies like dropout or early stopping to generalize better, especially when faced with noisy or imbalanced data.

* <h4><b> Data Files </b></h4> 

  - <b> Dataset for the project – </b> [Download Dataset]()
  - <b> Code for the project – </b> [View Code](https://github.com/Hamza-Siam/Hamza-Siam/blob/main/Extreme%20Learning%20Machine%20%26%20Multilayer%20Perceptron.pdf)
