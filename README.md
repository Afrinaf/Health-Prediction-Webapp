# Health Prediction WebApp

## Overview
Health Prediction WebApp is a machine learning-based web application that predicts various health conditions such as brain tumors, breast cancer, and performs sentiment analysis and speech recognition. Each model is trained using different datasets and provides predictions based on user input or uploaded files. The application is built using Flask and offers an intuitive web interface.

## Features
- **Brain Tumor Prediction**: Upload a brain MRI image, and the app predicts if a tumor is present using a pre-trained deep learning model.
- **Breast Cancer Prediction**: Based on medical data, the app predicts the likelihood of breast cancer using a machine learning model.
- **Sentiment Analysis**: Analyze the sentiment of a given text, showing positivity, negativity, and neutrality scores.
- **Speech Recognition**: Convert uploaded audio files to text using speech recognition techniques.

## Technologies Used
- **Python**: Core programming language.
- **Flask**: Web framework used for building the application.
- **TensorFlow/Keras**: For deep learning models like brain tumor prediction.
- **Scikit-learn**: For machine learning models (e.g., breast cancer prediction).
- **VADER**: For sentiment analysis.
- **SpeechRecognition**: For converting audio files to text.
- **HTML/CSS**: To create a user-friendly web interface.

## How to Use

### 1. Brain Tumor Prediction
1. Upload an MRI image of the brain.
2. The model processes the image and provides a prediction:
   - "You don't seem to have brain tumor!!"
   - "It seems like you have brain tumor."

### 2. Breast Cancer Prediction
1. Input medical data (age, BMI, glucose, etc.).
2. The machine learning model will provide a prediction on whether the user is at risk of breast cancer.

### 3. Sentiment Analysis
1. Input a block of text.
2. The sentiment analyzer will return the positivity, negativity, and neutrality scores along with a compound score.

### 4. Speech Recognition
1. Upload an audio file.
2. The app will convert the speech from the audio file into text using Google's speech recognition API.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/HealthPredictionWebApp.git
   cd HealthPredictionWebApp
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Download the required machine learning models and place them in the correct directories (e.g., `BrainTumor10Epochscategorical.h5` for brain tumor prediction).
4. Run the Flask application:
   ```bash
   python app.py
   ```
5. Open your browser and navigate to `http://127.0.0.1:5000/`.

## Models Used
- **Brain Tumor Prediction**: Pre-trained deep learning model (`BrainTumor10Epochscategorical.h5`) built using TensorFlow/Keras.
- **Breast Cancer Prediction**: Decision Tree Classifier (or similar) from Scikit-learn trained on medical data.
- **Sentiment Analysis**: VADER sentiment analyzer.
- **Speech Recognition**: Google Speech Recognition API for converting audio to text.

## Future Enhancements
- Improve the accuracy of the models with larger datasets and better training techniques.
- Add more health condition prediction features (e.g., diabetes, heart disease).
- Implement proper error handling for invalid inputs and missing files.
- Enhance the UI for a better user experience.

## License
This project is open-source and available under the MIT License.

