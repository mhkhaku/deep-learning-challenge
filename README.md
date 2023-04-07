# deep-learning-challenge

## Deep-learning Charity Evaluation Report

### Overview
Purpose of Analysis: To predict the success of a charity organization based on historic features of previous projects.

### Results
  - Data Preprocessing:
      - Target Variables: 'IS_SUCCESSFUL' feature, which is a binary value that indicates whether the money was used effectively or not

      - Features: All remaining columns other than the target column and the 'EIN' and 'NAME' columnms. The columns are increased to 44 after one-hot encoding

      - Removed Columns: EIN and NAME, they are neither targets nor features.

  - Compiling, Training, and Evaluating the Model

      - First Model Description:

        - Layers: 2

        - Nodes: 16, 8

        - epochs: 20

        - Activation Function: 'relu'

      - First Model Description:

         - Layers: 4

        - Nodes: 32, 16, 8, 4

        - epochs: 50

        - Activation Function: 'swish'

      - Results Accuracy:

        - First model: Accuracy: 72.5% Loss: 0.56

        - Second model: Accuracy: 72.9% Loss: 0.56

        - Target accuracy was not achieved

      - Optimization steps: The second model uses more nodes in the original 2 layers, adds 2 more layers, increases the epochs in addition to changing the activation function in an attempt to increase the accuracy.

### Summary
Although the second model shows a slight improvement in accuracy, the additional resources and processing time required do not justify its use. Instead, the Random Forest algorithm may be a better alternative. This machine learning model combines multiple decision trees to make predictions and is more interpretable, robust to noise and outliers, and quicker to train, making it more scalable. However, it's important to note that the best model for a particular problem and dataset can only be determined by comparing the performance of multiple models.
