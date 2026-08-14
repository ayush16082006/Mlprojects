# 🎓 Student Performance Prediction

A Machine Learning web application that predicts a student's **Math Score** based on demographic information, parental education, lunch type, test preparation, reading score, and writing score.

The machine learning model is integrated with a **Flask web application** and deployed online using **Render**.

---

## 🚀 Live Demo

🔗 **Live Application:**

https://mlprojects-x8b4.onrender.com

---

## 📌 Project Overview

The goal of this project is to predict a student's **Mathematics Score** using other available student performance attributes.

The application accepts the following inputs:

- Gender
- Race / Ethnicity
- Parental Level of Education
- Lunch Type
- Test Preparation Course
- Reading Score
- Writing Score

After submitting the information, the trained machine learning model predicts the student's **Math Score**.

---

## 🛠️ Technologies Used

### Programming Language

- Python

### Machine Learning

- Pandas
- NumPy
- Scikit-learn
- CatBoost
- XGBoost

### Web Development

- Flask
- HTML
- CSS

### Model Deployment

- Gunicorn
- Render

### Development Tools

- Git
- GitHub
- Postman
- VS Code

---

## 🤖 Machine Learning Workflow

The project follows a complete machine learning pipeline:

```text
Dataset
   ↓
Data Collection
   ↓
Data Preprocessing
   ↓
Exploratory Data Analysis
   ↓
Feature Engineering
   ↓
Model Training
   ↓
Model Evaluation
   ↓
Model Serialization
   ↓
Flask Application
   ↓
Postman API Testing
   ↓
Deployment on Render
```

---

## 📁 Project Structure

```text
MLProjects/
│
├── artifacts/
│   ├── model.pkl
│   └── preprocessor.pkl
│
├── src/
│   ├── components/
│   ├── pipeline/
│   │   └── pred_pipeline.py
│   ├── exception.py
│   ├── logger.py
│   └── util.py
│
├── templates/
│   ├── home.html
│   └── ...
│
├── app.py
├── requirements.txt
├── .python-version
├── .gitignore
└── README.md
```

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/ayush16082006/Mlprojects.git
```

### 2. Navigate to the project directory

```bash
cd mlprojects
```

### 3. Create a virtual environment

```bash
python -m venv venv
```

### 4. Activate the virtual environment

For Windows:

```bash
venv\Scripts\activate
```

### 5. Install the required dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Application Locally

Start the Flask application:

```bash
python app.py
```

The application will run at:

```text
http://127.0.0.1:5000
```

Open the URL in your browser and enter the required student information.

---

## 🔌 API Testing with Postman

The prediction endpoint can also be tested using **Postman**.

### Prediction Endpoint

```text
POST /predictdata
```

### Example Input

```text
gender: male
race_ethnicity: group B
parental_level_of_education: bachelor's degree
lunch: standard
test_preparation_course: completed
reading_score: 75
writing_score: 80
```

The input is processed by the preprocessing pipeline and passed to the trained machine learning model.

The API then returns the predicted **Math Score**.

---

## 🧠 Machine Learning Pipeline

The prediction pipeline works as follows:

```text
User Input
    ↓
CustomData
    ↓
Pandas DataFrame
    ↓
Preprocessor
    ↓
Feature Transformation
    ↓
Trained ML Model
    ↓
Math Score Prediction
```

The trained model and preprocessing object are stored in the `artifacts` directory:

```text
artifacts/
├── model.pkl
└── preprocessor.pkl
```

---

## 📦 Requirements

The project uses the following dependencies:

```text
numpy
pandas
seaborn
matplotlib
scikit-learn==1.3.2
catboost
xgboost
dill
Flask
gunicorn
```

### Important

The project uses:

```text
scikit-learn==1.3.2
```

because the saved machine learning model and preprocessing objects were created using this version of scikit-learn.

The project also specifies Python:

```text
3.10.11
```

in the `.python-version` file for deployment compatibility.

---

## 🌐 Deployment

The application is deployed using **Render**.

The deployment workflow is:

```text
GitHub Repository
        ↓
Render
        ↓
Install Dependencies
        ↓
Build Application
        ↓
Gunicorn
        ↓
Flask Application
        ↓
Live Website
```

The production server uses Gunicorn to run the Flask application.

---

## 🧪 Testing

The application was tested using:

- Local Flask server
- Web browser
- Postman
- Render production deployment

The deployed application successfully accepts student information and generates a predicted Math Score.

---

## 🔮 Future Improvements

Possible improvements include:

- Improve model accuracy
- Compare multiple machine learning algorithms
- Add model performance visualizations
- Improve the user interface
- Add prediction history
- Add user authentication
- Create additional REST API endpoints
- Add automated testing
- Add monitoring for the deployed application

---

## 👨‍💻 Author

**Ayush Kumar**

Computer Science & Engineering – Data Science

---

## ⭐ Project Highlights

- End-to-end Machine Learning project
- Data preprocessing pipeline
- Machine learning model training
- Model serialization
- Flask web application
- REST API testing using Postman
- Git and GitHub integration
- Production deployment using Render
- Live prediction system

---

## 🔗 Project Links

### Live Application

https://mlprojects-x8b4.onrender.com

### GitHub Repository

https://github.com/ayush16082006/Mlprojects