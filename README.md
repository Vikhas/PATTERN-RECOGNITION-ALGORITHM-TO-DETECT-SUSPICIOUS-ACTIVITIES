---

# PATTERN RECOGNITION ALGORITHM TO DETECT SUSPICIOUS ACTIVITIES

## Abstract

Detecting suspicious activities in public places with high foot traffic is increasingly critical due to rising crime rates and incidents. The challenge lies in the unpredictable nature of human behavior, which complicates reliable monitoring. Continuous human supervision across multiple screens is impractical, making automated surveillance systems essential. This project proposes a solution that leverages object detection models and high-resolution cameras to identify potential threats, such as explosions, accidents, or possession of weapons. The system uses machine learning techniques for pattern recognition to detect anomalies and alert monitoring authorities. The project evaluates various object detection algorithms to determine the most effective model based on performance metrics.

## Overview

This repository contains a web application that uses a saved model to make predictions on uploaded videos. The application is built with Flask and provides a web interface for interacting with the model.

## Directory Structure

- **Suspicious Activity Code/application/**: Contains the saved model and Flask API for the web application.
  - **unsus_keras.pb**: Directory containing the saved model.
  - **Flask/**: Contains the Flask app and static files.
    - **static/files/frames/**: Directory for storing image frames extracted from uploaded videos.
    - **main.py**: Main entry point for running the Flask application.

- **Suspicious Activity Code/codes/**: Contains Colab notebooks used for model creation.
  - **unsus_keras.pynb**: Colab notebook for the first model.
  - **unsus_mobile.pynb**: Colab notebook for the second model.

## Getting Started

### Prerequisites

Ensure you have Python and the necessary libraries installed. Use `pip` to install the required packages.

### Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/your-username/your-repository.git
   cd your-repository
   ```

2. **Install Dependencies**

   Install the required Python packages using `requirements.txt`:

   ```bash
   pip install -r requirements.txt
   ```

### Steps for Executing the Application

1. **Extract the Application Folder**

   Extract the contents of the `application` folder to your local machine.

2. **Configure Model Path**

   Update the path for loading the model in `main.py` to match the directory on your machine:

   ```python
   model_path = 'path_to_your_model/unsus_keras.pb'
   ```

3. **Run the Flask Application**

   Start the Flask application by running:

   ```bash
   python main.py
   ```

   You will receive a URL where the app is hosted.

4. **Access the Web Application**

   Open your browser and navigate to the URL provided by the Flask app. The home page will be displayed.

5. **Upload Video**

   Click the "Add File" button to upload the video you want to analyze.

6. **Submit for Prediction**

   Click the "Submit" button after uploading. The application will process the video and redirect you to the result page.

7. **View Results**

   On the result page, you will see the type of suspicious activity detected in the video based on the model’s prediction.

## Colab Notebooks

The `codes` directory contains Colab notebooks used for model creation:

- **unsus_keras.pynb**: Contains the code for the first model.
- **unsus_mobile.pynb**: Contains the code for the second model.
  
---
