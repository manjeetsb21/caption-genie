

# Image Captioning Web Application with Flask and MySQL

This repository contains a web application built using Flask that allows users to generate captions for images and provide feedback on the results. The application implements an advanced image captioning model and stores user reviews securely in a MySQL database.

## Project Overview

The project aims to provide an interactive interface for users to generate detailed image captions using the **IdeficsForVisionText2Text** model. The system collects user feedback and securely stores it in a MySQL database for future analysis. The model's performance is optimized for efficiency and deployed on Hugging Face's Model Hub for easy access and scalability.

### Key Features:

- **Image Captioning**: Implemented advanced image captioning using IdeficsForVisionText2Text, with image preprocessing and high-quality text generation.
- **User Interface**: Developed a user-friendly interface using Flask for uploading images, generating captions, and submitting reviews.
- **Database Integration**: Securely stored user feedback in a MySQL database, ensuring data integrity and accessibility for analysis.
- **Model Optimization**: Enhanced model performance using 4-bit quantization and Low-Rank Adaptation (LoRA), optimizing both training and inference efficiency.
- **Deployment**: Configured and deployed the model to Hugging Face's Model Hub for seamless integration and scalability.

## Installation

### Prerequisites

- Python 3.x
- Flask
- MySQL
- Hugging Face Transformers and Datasets Libraries

### Setup

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/image-captioning-flask.git
   cd image-captioning-flask
   ```

2. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Set up the MySQL database:
   - Create a database in MySQL.
   - Import the SQL file from the `/database` directory.
   - Update the database connection details in `config.py`.

4. Run the Flask application:
   ```bash
   python app.py
   ```

## Usage

- **Upload Image**: Users can upload images through the web interface.
- **Generate Caption**: The application processes the image and generates a detailed caption using the IdeficsForVisionText2Text model.
- **Submit Feedback**: Users can provide feedback on the generated captions, which will be securely stored in the MySQL database.

## Model Optimization

- **4-bit Quantization**: Applied 4-bit quantization to reduce model size and improve inference efficiency without sacrificing accuracy.
- **LoRA (Low-Rank Adaptation)**: Used LoRA for fine-tuning, optimizing memory usage and computational efficiency during model training.

## Deployment

The model is deployed on Hugging Face's Model Hub, allowing for easy access and integration into the Flask application. The deployment configuration was handled using AutoProcessor and TrainingArguments.


