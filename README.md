# Gait Authentication System

## Project Overview

This project implements an AI-powered gait authentication system using deep learning models to verify employee identities based on their walking patterns. The system utilizes accelerometer and gyroscope data from smartphones to authenticate employees securely.

## Features

- Real-time employee authentication based on gait patterns
- Supports LSTM and CNN-LSTM deep learning models
- User-friendly Gradio-based interface for authentication
- Live visualization of accelerometer and gyroscope data
- High accuracy in distinguishing individuals based on walking patterns

## Technologies Used

- Python
- TensorFlow / Keras
- Scikit-learn
- Pandas, NumPy, Matplotlib
- Gradio for UI
- Google Colab for training

## Dataset

The model is trained on raw accelerometer and gyroscope data collected using the Physics Toolbox Sensor Suite app. The dataset consists of:

- `body_gyro_x.csv`, `body_gyro_y.csv`, `body_gyro_z.csv`
- `total_acc_x.csv`, `total_acc_y.csv`, `total_acc_z.csv`

Real-time test data is collected from employees' smartphones and processed for authentication.

## Setup Instructions

### Clone the Repository

```sh
git clone https://github.com/your-username/gait-authentication.git  
cd gait-authentication  
```

### Install Dependencies

```sh
pip install -r requirements.txt  
```

### Extract Dataset

```sh
python extract_data.py  
```

### Train the Authentication Model

```sh
python train_model.py  
```

### Run the Gradio Web Interface

```sh
python app.py  
```

Access the authentication system at `http://localhost:7860/`.

## Model Training

- The LSTM model is trained on preprocessed gait data.
- The dataset is standardized using `StandardScaler`.
- The model achieves high accuracy in recognizing employees based on gait patterns.

## Model Performance

The best model achieved **90% accuracy** on real-world gait authentication.

| Model    | Accuracy |
| -------- | -------- |
| LSTM     | 87.5%    |
| CNN-LSTM | 90.2%    |

## Deployment

The project can be deployed using Gradio or hosted on Hugging Face Spaces.











