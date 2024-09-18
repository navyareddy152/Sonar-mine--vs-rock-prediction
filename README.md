**Sonar Object Classification Using Logistic Regression**
**Overview**
This project uses a logistic regression model to classify objects as either a Mine or Rock based on Sonar return data. The dataset consists of 60 features extracted from sonar signals, which are used to train the model.

**Project Features**
Data Loading and Preprocessing:

The dataset is loaded from a CSV file without a header.
Labels are separated from the feature data.
**Model Training:**

The model is trained using Logistic Regression.
The dataset is split into training and test sets.
**Model Evaluation:**

Model accuracy is calculated on both training and test data.
**Prediction:**

A predictive system is built to classify new input data as either Mine or Rock.
**Dataset**
The dataset used in this project contains 60 features for each sample and one label indicating if the object is a Mine or Rock.
Dataset file: sonar data.csv
**Requirements**
_Install the following libraries:_
pip install numpy pandas scikit-learn
**Project Structure**
Data collection: The dataset is loaded using pandas and statistics about the data are explored.
Training and test data splitting: The data is split using train_test_split with stratification to maintain label distribution.
Model training: A logistic regression model is trained on the sonar data.
Evaluation: The model's accuracy is checked on both training and testing datasets.
Prediction: The model is tested with a sample input to predict whether it represents a mine or rock.

Follow these steps in the notebook:

Load the dataset
Preprocess the data
Train the model
Evaluate the model
Use the prediction system for new inputs.
Model Accuracy
Training Data Accuracy: Achieves an accuracy of around [83.4] on the training data.
Test Data Accuracy: Achieves an accuracy of around [76.19] on the test data.
**Prediction Example**

input_data = (0.0117, 0.0069, 0.0279, 0.0583, ...)
prediction = model.predict(input_data_reshaped)

if(prediction[0]=='R'):
    print('The object is a rock')
else:
    print('The object is a mine')
**Conclusion**
This project demonstrates the use of logistic regression for classifying sonar data into two classes: Mine or Rock. With a reasonable accuracy, the model can predict the class of new inputs based on 60 sonar features.
