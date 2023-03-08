# deep-learning-challenge

https://colab.research.google.com/drive/1g4VK5SUOUhfMpHrC9c5cae2A3apWka8B?usp=sharing

https://colab.research.google.com/drive/1W_VZzK1ImPeG0RBW4-T7eyG31nHXqikx?usp=sharing

Alphabet Soup Charity Optimization
This code implements a neural network model to predict whether applicants will be successful if funded by Alphabet Soup Charity. It utilizes hyperparameter tuning using the Keras Tuner package to optimize the model's performance.

Getting Started
To run the code, the following dependencies must be imported:

sklearn
pandas
tensorflow
google.colab
keras-tuner
The input data is stored in the Google Drive in CSV format. The data can be read using pandas and the URL to the CSV file.

Data Preprocessing
After importing the data, the non-beneficial columns EIN and NAME are dropped. The number of unique values in each column is determined. Next, categorical data is converted to numeric data using pd.get_dummies(). The preprocessed data is split into features and target arrays, and then the data is scaled using StandardScaler.

Creating a Neural Network Model
The create_model() function is defined to create a neural network model with hyperparameters defined by Keras Tuner. The keras-tuner package is imported and kt.RandomSearch() is used to search for the best hyperparameters. The max_trials parameter specifies the number of models to be tested. The objective parameter specifies the metric to optimize. The directory parameter specifies the path to the directory to save search results, and project_name specifies the name of the project. The search() method is then called to search for the best hyperparameters, and the results_summary() method is called to print a summary of the results.

Evaluating the Model
The best hyperparameters are obtained using tuner.get_best_hyperparameters(), and the best models are obtained using tuner.get_best_models(). The top three hyperparameters and models are printed to the console, and the best model is used to make predictions on the test data. The model's accuracy and loss are printed to the console. Finally, the best model is saved to an HDF5 file.


https://colab.research.google.com/drive/1g4VK5SUOUhfMpHrC9c5cae2A3apWka8B?usp=sharing

https://colab.research.google.com/drive/1W_VZzK1ImPeG0RBW4-T7eyG31nHXqikx?usp=sharing
