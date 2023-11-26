# Sentiment Analysis Web App using PyTorch and SageMaker

## Overview

This project, completed as part of the Deep Learning Nanodegree Program, demonstrates the end-to-end process of creating a sentiment analysis web app. The goal is to allow users to input a movie review on a web page, which is then sent to a deployed PyTorch model on Amazon SageMaker for sentiment prediction.

## General Outline

1. **Data Processing:**
   - Download or retrieve the movie review dataset.
   - Process and prepare the data.
   - Upload the processed data to Amazon S3.

2. **Build and Train the PyTorch Model:**
   - Construct a PyTorch model.
   - Train the model using the processed data.

3. **Testing the Model:**
   - Deploy the trained model on SageMaker.
   - Test the deployed model by sending test data to the endpoint.

4. **Deploy Model for Web App:**
   - Customize the model deployment with additional code.
   - Deploy the trained model for a second iteration.

5. **Web App Interaction:**
   - Create a Lambda function for processing reviews.
   - Set up API Gateway to trigger the Lambda function.
   - Deploy the web app, allowing users to interact with the SageMaker model.

## Instructions

The project includes Jupyter Notebooks, Python scripts, and HTML files. Instructions for each step are provided in the respective sections of the notebooks. Additionally, questions are posed throughout the notebooks for reflection and understanding.

**Note:** Make sure to manage the lifecycle of the deployed SageMaker endpoint. Shut it down when not in use to avoid unnecessary costs.

## File Structure

- **data_processing.ipynb:** Notebook for processing and preparing the movie review dataset.
- **train_model.ipynb:** Notebook for building, training, and testing the PyTorch model.
- **deploy_model.ipynb:** Notebook for deploying and testing the model in SageMaker.
- **website/index.html:** HTML file for the simple web app.
- **serve/predict.py:** Python script containing custom inference code for model deployment.
- **train/model.py:** Implementation of the PyTorch model.

## How to Use

1. Open and run the notebooks sequentially:
   - data_processing.ipynb
   - train_model.ipynb
   - deploy_model.ipynb

2. Deploy the web app:
   - Replace the placeholder in website/index.html with the actual API endpoint URL.
   - Host the HTML file on a web server (e.g., GitHub Pages, S3).

3. Interact with the web app:
   - Input movie reviews and observe sentiment predictions.

4. Manage SageMaker endpoint:
   - Shut down the SageMaker endpoint when not in use to avoid unnecessary costs.

## Conclusion

This project showcases the integration of PyTorch, SageMaker, Lambda, and API Gateway to create a sentiment analysis web app. The provided materials serve as an educational resource for those interested in deploying machine learning models for real-world applications.
