**Sonar Object Classification Using Logistic Regression**
**Overview**<br/>
This project uses a logistic regression model to classify objects as either a Mine or Rock based on Sonar return data. The dataset consists of 60 features extracted from sonar signals, which are used to train the model.<br/>

**Project Features**<br/>
Data Loading and Preprocessing:<br/>
- The dataset is loaded from a CSV file without a header.<br/>
- Labels are separated from the feature data.<br/>
**Model Training** <br/>
- The model is trained using Logistic Regression.
- The dataset is split into training and test sets.
**Model Evaluation:** <br/>
Model accuracy is calculated on both training and test data.<br/>
**Prediction:** <br/>
A predictive system is built to classify new input data as either Mine or Rock. <br/>
**Dataset** <br/>
The dataset used in this project contains 60 features for each sample and one label indicating if the object is a Mine or Rock.<br/>
Dataset file: copy of sonar data.csv <br/>
**Requirements** <br/>
_Install the following libraries:_<br/>
pip install numpy pandas scikit-learn <br/>
**Project Structure** <br/>
Data collection: The dataset is loaded using pandas and statistics about the data are explored. <br/>
Training and test data splitting: The data is split using train_test_split with stratification to maintain label distribution. <br/>
Model training: A logistic regression model is trained on the sonar data. <br/>
Evaluation: The model's accuracy is checked on both training and testing datasets. <br/>
Prediction: The model is tested with a sample input to predict whether it represents a mine or rock. <br/>

Follow these steps in the notebook: <br/>

1. Load the dataset
2. Preprocess the data
3. Train the model
4. Evaluate the model
5. Use the prediction system for new inputs.
6. Model Accuracy
7. Training Data Accuracy: Achieves an accuracy of around [83.4] on the training data.
8. Test Data Accuracy: Achieves an accuracy of around [76.19] on the test data. <br/>
**Prediction Example** <br/>

input_data = (0.0117, 0.0069, 0.0279, 0.0583, ...) 
prediction = model.predict(input_data_reshaped) 

if(prediction[0]=='R'):
    print('The object is a rock')
else:
    print('The object is a mine') <br/>
**Conclusion** <br/>
This project demonstrates the use of logistic regression for classifying sonar data into two classes: Mine or Rock. With a reasonable accuracy, the model can predict the class of new inputs based on 60 sonar features. 
