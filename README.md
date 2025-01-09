```markdown
# Breast Cancer Predictor

This application is a Streamlit-based web app designed to help diagnose breast cancer. It uses machine learning to predict whether a breast mass is benign or malignant based on cell nuclei measurements. 

## Features

- **Interactive Sidebar**: Modify input values using sliders in the sidebar to update predictions dynamically.
- **Visualization**: Generates a radar chart to visualize scaled measurements for mean, standard error, and worst-case values.
- **Machine Learning Predictions**: Uses a pre-trained model to provide predictions and probabilities for benign and malignant diagnoses.

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-repo/breast-cancer-predictor.git
   cd cancer-predictor-app
   ```

2. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. Ensure the following files are in place:
   - Data file: `data/data.csv`
   - Model file: `model/model.pkl`
   - Scaler file: `model/scaler.pkl`

## Usage

Open the Website: https://cancer-prediction-2025.streamlit.app/


## File Structure

- `app.py`: Main application script.
- `data/data.csv`: Dataset containing cell nuclei measurements.
- `model/model.pkl`: Pre-trained machine learning model for predictions.
- `model/scaler.pkl`: Scaler object for feature normalization.

## How It Works

1. **Data Preprocessing**: The app reads and cleans data from `data/data.csv`, mapping the diagnosis column to binary values (1: Malignant, 0: Benign).
   
2. **Sidebar Input**: Users can modify cell nuclei measurement values using sliders in the sidebar.

3. **Prediction**: Input data is scaled, and the pre-trained model predicts whether the mass is benign or malignant. The app also displays the probabilities for each class.

4. **Radar Chart**: A radar chart visualizes the scaled values of different measurements for mean, standard error, and worst-case scenarios.

## Requirements

- Python 3.7+
- Libraries:
  - `streamlit`
  - `pandas`
  - `numpy`
  - `plotly`
  - `scikit-learn`

## Credits

This app was created to assist in diagnosing breast cancer using machine learning and interactive data visualization. 

## Disclaimer

This application is for educational purposes only and should not be used as a substitute for professional medical advice. Always consult a qualified healthcare provider for diagnosis and treatment.
