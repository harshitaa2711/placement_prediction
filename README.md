Dataset: https://www.kaggle.com/datasets/sevdanurgenc/placement-data-full-class

# **Campus Placement Prediction App**

This is a simple web-based application built using **Flask** that predicts the likelihood of a student getting placed based on various academic factors. The app takes user inputs through a form, runs predictions using a pre-trained model, and displays the result along with the probability of placement.

## **Features**

- **Input Features**: The user provides their details such as:
  - Gender
  - Specialization
  - Technical Skills
  - Work Experience
  - Academic scores (SSC, HSC, DSC, MBA)
  
- **Model**: The app uses a pre-trained **Random Forest Classifier** model (`campusplacementpredictor.pkl`) to predict the likelihood of placement.

- **Output**: The app outputs whether the student is likely to be placed or not and provides the probability percentage.

## **Tech Stack**
- **Flask**: For building the web application.
- **Pickle**: For loading the pre-trained model.
- **HTML/CSS**: For the front-end user interface.

## **How It Works**

1. When you run the app, you will be presented with an input form on the home page (`index.html`).
2. Fill in the details such as gender, specialization, technical skills, work experience, and academic scores.
3. After submitting the form, the app will use the trained model to predict whether the student is likely to be placed or not.
4. The result will be displayed with the probability of placement on a new page (`show.html`).

## **Setup Instructions**

To run the app locally, follow the steps below:

### 1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/placement-prediction-app.git
   cd placement-prediction-app
   ```

### 2. **Install dependencies**
   You need Python 3.7+ and pip installed.

   Install the required Python libraries:

   ```bash
   pip install -r requirements.txt
   ```

   If you don't have the `requirements.txt` file, you can manually install the dependencies:

   ```bash
   pip install Flask
   pip install pickle
   ```

### 3. **Run the app**

   ```bash
   python app.py
   ```

   The app will start running locally on `http://127.0.0.1:5000/`. Open this URL in your browser to interact with the app.

### 4. **Model File**

   Make sure the **`campusplacementpredictor.pkl`** model file is placed in the same directory as your app.

## **Folder Structure**

```
placement-prediction-app/
│
├── app.py                    # Main Flask application
├── campusplacementpredictor.pkl   # Trained model
├── templates/
│   ├── index.html            # Home page with form
│   └── show.html             # Display prediction results
└── requirements.txt          # Python dependencies (optional)
```

