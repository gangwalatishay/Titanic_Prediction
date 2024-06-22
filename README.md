**Titanic Survival Prediction**
This repository contains a machine learning model built with Logistic Regression to predict survival on the Titanic based on various passenger attributes. The model is deployed using Flask and accessible via a web interface.

**Project Structure**
**train.csv**: Dataset used to train the machine learning model.
**logistic_regression_model.pkl**: Serialized Logistic Regression model saved using joblib.
**app.py**: Flask application for serving the prediction model.
**templates/:
index.html**: HTML template for the web interface to collect user inputs.

README.md: Detailed documentation about the project.


**Getting Started**
To get a local copy up and running, follow these steps:

**Prerequisites**
**Python 3.x**
Pip (Python package installer)
Installation
**Clone the repo:**
sh
Copy code
git clone https://github.com/your_username/repo_name.git
**Navigate to the project directory:**
sh
Copy code
cd repo_name
**Install dependencies:**
sh
Copy code
pip install -r requirements.txt
**Usage**
Start the Flask application:
sh
Copy code
python app.py
This will start the Flask server locally.

**Open your browser and go to http://127.0.0.1:5000 to access the web interface**.
Enter passenger details (Pclass, Sex, Age, SibSp, Parch, Fare, Embarked) and click Predict to see the survival prediction.

**Features**
**Machine Learning Model**
**Logistic Regression Model**: Trained using the Titanic dataset (train.csv) to predict survival probabilities based on passenger attributes such as:
**Pclass**: Ticket class (1st, 2nd, 3rd).
**Sex:** Gender of the passenger (male or female).
**Age**: Age of the passenger.
**SibSp**: Number of siblings/spouses aboard.
**Parch**: Number of parents/children aboard.
**Fare**: Passenger fare.
**Embarked**: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton).

**Web Application**
**Flask Backend**: Implements the prediction model using Flask, a Python web framework.
**HTML Form**: Provides a user-friendly interface for entering passenger details.
**Real-time Prediction**: Users can input the aforementioned attributes and receive a prediction on whether a passenger would survive the Titanic disaster.

**Deployment**
**Ngrok Integration**: Sets up a secure tunnel to expose the local Flask server to the internet, allowing remote access to the prediction service.
**Public URL**: Generates a public URL using Ngrok, making the application accessible from anywhere.

**Data Handling and Preprocessing**
**Data Loading**: Loads the Titanic dataset (train.csv) using pandas for training the model.
**Data Preprocessing**:
Handles missing values in the dataset (e.g., filling missing ages with the mean age).
Encodes categorical variables (e.g., converting 'Sex' and 'Embarked' to numeric values).
Splits the dataset into training and testing sets using train_test_split from scikit-learn.

**Model Evaluation**
**Accuracy Metrics**: Calculates and displays accuracy scores for both training and testing datasets to evaluate model performance.

**File Structure**
**train.csv**: Raw dataset used for training the machine learning model.
**logistic_regression_model.pkl**: Serialized Logistic Regression model saved using joblib for deployment.
**app.py**: Flask application handling HTTP requests and serving predictions.
**templates/:
index.html**: HTML template for the web interface to collect user inputs.
**Usage**

**Local Deployment:**
Clone the repository, install dependencies, and run app.py to start the Flask server locally.
Access the web interface at http://127.0.0.1:5000 to input passenger details and get survival predictions.
Remote Access:

Utilize Ngrok to create a secure tunnel to expose the local Flask server.
Share the generated public URL to allow others to access and use the prediction service remotely.

**Contributions are welcome! If you wish to improve the project, add features, or fix issues, please fork the repository, create a new branch, and submit a pull request.**


**Web Interface**
The web interface provides a form where users can input passenger details. Upon submission, the Flask backend uses the trained Logistic Regression model to predict whether the passenger survived the Titanic disaster.

**Additional Notes**
The model was trained using the Titanic dataset (train.csv). It handles missing values and encodes categorical variables before training.
Accuracy metrics (both training and testing) are provided to assess model performance.
Ngrok is used to create a secure tunnel to expose the local Flask server to the internet, making the prediction service accessible remotely.
Contributing Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are greatly appreciated.

**Fork the Project**
Create your Feature Branch (git checkout -b feature/AmazingFeature)
Commit your Changes (git commit -m 'Add some AmazingFeature')
Push to the Branch (git push origin feature/AmazingFeature)
Open a Pull Request

**Contact**
Atishay Gangwal -  jatishay057@gmail.com

**Project Link**: https://github.com/gangwalatishay/Titanic_Prediction

**Acknowledgements**
Pyngrok for creating tunnels to expose local servers.
Flask for building the web application.
Seaborn and Matplotlib for data visualization.
Scikit-learn for machine learning tools.

 
 Happy coding!
