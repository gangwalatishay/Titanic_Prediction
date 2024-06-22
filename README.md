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
