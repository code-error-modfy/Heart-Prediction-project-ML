# Heart Disease Prediction Application

## Main Concept

The **Heart Disease Prediction Application** leverages machine learning, specifically logistic regression, to predict the likelihood of heart disease based on various health metrics. This application serves as both a practical tool for risk assessment and an educational resource for understanding the factors influencing heart disease.

### Key Components

1. **Machine Learning Model**
   - **Logistic Regression**: A statistical method used for binary classification, predicting whether a patient has heart disease (1) or not (0) based on input features.

2. **Input Features**
   The application accepts the following health metrics from users:
   - **Age**: Patient's age in years.
   - **Sex**: Gender of the patient (1 for male, 0 for female).
   - **Chest Pain Type**: Categorized into four types (0-3).
   - **Resting Blood Pressure**: Measurement in mm Hg.
   - **Cholesterol**: Serum cholesterol levels in mg/dl.
   - **Fasting Blood Sugar**: Binary value indicating if fasting blood sugar is greater than 120 mg/dl.
   - **Resting Electrocardiographic Results**: Evaluation of heart's electrical activity.
   - **Maximum Heart Rate Achieved**: Highest heart rate during exercise.
   - **Exercise-Induced Angina**: Indicator of angina during exercise (1 for yes, 0 for no).
   - **Oldpeak**: Depression of ST segment during exercise.
   - **Slope**: Slope of the peak exercise ST segment (0: upsloping, 1: flat, 2: downsloping).
   - **Number of Major Vessels**: Count of colored blood vessels (0-3).
   - **Thalassemia**: Categorical feature representing different types of thalassemia.

3. **Data Preprocessing**
   - Loads a heart disease dataset, splits it into training and testing sets, and standardizes the input features to enhance model performance.

4. **User Interface**
   - Built using **Tkinter**, the application provides a graphical user interface (GUI) for users to enter health metrics, view predictions, and understand the features affecting heart disease risk.
   - Includes buttons for submitting data, clearing input fields, and exiting the application.

5. **Prediction Output**
   - After submission of health metrics, the model predicts the likelihood of heart disease and displays the result clearly to the user.

6. **Educational Aspect**
   - Features an explanation section detailing each input feature, promoting user understanding of the health metrics involved in heart disease risk.

7. **Real-World Implication**
   - Aims to raise awareness and encourage users to seek medical advice based on their health data, potentially leading to earlier detection and intervention of heart disease.


# Architecture of Heart Disease Prediction Application

## Overview

The architecture of the Heart Disease Prediction Application is structured to efficiently handle user inputs, process data, and provide predictions using machine learning. It consists of distinct layers, ensuring separation of concerns for maintainability and scalability.

## Architecture Components

### 1. User Interface Layer
- **Framework**: Tkinter
- **Responsibilities**:
  - Provides a graphical user interface (GUI) for user interaction.
  - Displays input fields, prediction results, and explanations.

### 2. Application Logic Layer
- **Responsibilities**:
  - Manages data flow between the GUI and the machine learning model.
  - Validates user inputs and handles events triggered by user actions.

### 3. Machine Learning Layer
- **Model**: Logistic Regression
- **Framework**: scikit-learn
- **Responsibilities**:
  - Loads the heart disease dataset for training and testing.
  - Preprocesses data (scaling and splitting).
  - Trains the model and makes predictions based on user inputs.

### 4. Data Management Layer
- **Data Source**: CSV File
- **Responsibilities**:
  - Loads and preprocesses heart disease data.
  - Stores the trained model for making predictions.

## Data Flow

1. **User Input**: Users enter health metrics through the GUI.
2. **Data Validation**: The application logic checks for valid inputs.
3. **Data Preprocessing**: Validated data is prepared for the machine learning model.
4. **Prediction**: The model predicts the likelihood of heart disease.
5. **Display Result**: The prediction result is shown on the GUI.


# Tkinter in Heart Disease Prediction Application

## Overview

Tkinter is the standard GUI (Graphical User Interface) toolkit for Python. It provides a simple and efficient way to create interactive applications. In the Heart Disease Prediction Application, Tkinter is used to build the user interface, allowing users to enter their health metrics and receive predictions about heart disease.

## Key Features of Tkinter Used in the Application

### 1. Window Management
- **Main Window**: The application creates a main window that serves as the container for all other UI elements.
- **Geometry**: The window size and position are configured to provide an optimal user experience.

### 2. Widgets
- **Labels**: Used to display text, such as input prompts and explanations of health metrics.
- **Entry Fields**: Input fields where users enter their health data, allowing for interactive data collection.
- **Buttons**: 
  - **Submit**: Triggers the prediction process based on the user inputs.
  - **Clear**: Resets all input fields and clears any displayed predictions.
  - **Exit**: Closes the application.

### 3. Layout Management
- **Pack Geometry Manager**: Utilizes the `pack()` method to arrange widgets vertically, ensuring a clean and organized interface.
- **LabelFrame**: Groups related widgets (like explanations) for better organization and clarity.
- **Sticky Note-like Widget**: A scrolled text area that acts as a sticky note for displaying predictions and messages, enhancing user interaction.

### 4. User Interaction
- **Event Handling**: Tkinter handles user inputs and button clicks, invoking the appropriate functions for data processing and prediction.
- **Message Boxes**: Displays error messages or prediction results using Tkinter's built-in message box functionality.

# References

1. **Scikit-learn Documentation**: 
   - The official documentation for scikit-learn, a machine learning library in Python, provides comprehensive guides and API references for implementing machine learning algorithms.
   - [Scikit-learn](https://scikit-learn.org/stable/documentation.html)

2. **Pandas Documentation**: 
   - The official documentation for Pandas, a data manipulation and analysis library for Python, which is used for data preprocessing in this application.
   - [Pandas](https://pandas.pydata.org/docs/)

3. **Tkinter Documentation**: 
   - The official Python documentation for Tkinter, which provides details on how to create graphical user interfaces in Python.
   - [Tkinter](https://docs.python.org/3/library/tkinter.html)

4. **Logistic Regression**: 
   - A brief overview of logistic regression, including its mathematical foundation and applications in binary classification.
   - [Logistic Regression](https://en.wikipedia.org/wiki/Logistic_regression)

5. **Heart Disease Data Set**: 
   - Description of the dataset used for training the model, which can typically be found on platforms like UCI Machine Learning Repository or Kaggle.
   - [UCI Machine Learning Repository - Heart Disease Data Set](https://archive.ics.uci.edu/ml/datasets/heart+Disease)

6. **Python Documentation**: 
   - The official Python documentation provides extensive resources for Python programming.
   - [Python](https://docs.python.org/3/)

## Acknowledgments

- Special thanks to the contributors and developers of the libraries used in this project, as well as to the community for shared knowledge and resources that made this application possible.

## Output
![Screenshot (155)](https://github.com/user-attachments/assets/e5e39cdd-f2e0-4f73-8e4f-5a32f0c60b70)
![Screenshot (156)](https://github.com/user-attachments/assets/3504b388-26fb-430c-8e00-eccffa2767e1)
![Screenshot (157)](https://github.com/user-attachments/assets/1f1f394b-3c95-413b-9f50-19aa66c10dcc)
### Conclusion

The Heart Disease Prediction Application combines machine learning techniques with a user-friendly interface, empowering individuals to assess their heart health based on established medical metrics.
