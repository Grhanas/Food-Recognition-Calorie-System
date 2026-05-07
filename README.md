# AI-Supported Food Recognition and Calorie Estimation

This repository summarizes an undergraduate graduation thesis project focused on building an AI-supported mobile application for food recognition and calorie estimation.

The main goal of the project was to reduce the need for manual food entry by allowing users to take or upload food images, detect the food items using a computer vision model, and estimate calorie values through a mobile application interface.

## Project Overview

The project combines deep learning-based object detection, mobile application development, and calorie estimation logic. The system is designed to recognize food items from images and support users in tracking their daily calorie intake more easily.

The application workflow can be summarized as follows:

1. The user takes a food photo or selects one from the gallery.
2. The trained object detection model analyzes the image.
3. Detected food items are matched with calorie-related information.
4. The estimated calorie value is displayed in the mobile application.
5. Users can also track or manually update their daily calorie intake.

## Motivation

Traditional calorie tracking applications often require users to manually enter every consumed food item. This can be time-consuming and error-prone.

This project aimed to make the process more practical by using artificial intelligence and image-based food recognition. The final system was designed to help users monitor their nutrition habits and make more informed decisions about their daily food consumption.

## Machine Learning Approach

The project used a YOLOv8 Nano object detection model for food recognition. YOLOv8n was selected because it provides a good balance between detection performance and computational efficiency, which is especially important for mobile deployment.

The model was trained and tested in Google Colab. After training, the model was converted into TensorFlow Lite format so that it could be integrated into a mobile application.

## Dataset Design

Different dataset scenarios were considered to improve the model's generalization ability:

- Single food type images
- Multiple plates in the same image
- Multiple food types on a single plate
- Images captured from different angles
- Different portion sizes
- Different plate types
- Images with noise and real-world side objects such as forks, spoons, hands, or phones

This dataset strategy was used to make the model more robust for realistic user scenarios.

## Mobile Application

A mobile application interface was designed to make the AI model usable by end users. The app included:

- Home screen for taking or selecting food images
- Model prediction screen
- User profile screen
- Daily calorie tracking screen
- Manual calorie entry and update screens

The trained model was converted to TensorFlow Lite and integrated into the mobile application so that predictions could be performed in a mobile environment.

## Calorie Estimation Logic

In addition to food recognition, the project proposed a calorie estimation approach based on detected food information and volume-to-weight relationships.

The idea was to estimate food quantity using visual information and then calculate calorie values using food-specific calorie data. The project also included user-related calorie calculations such as daily calorie needs based on profile information.

## Tech Stack

- Python
- YOLOv8n
- Computer Vision
- Object Detection
- Google Colab
- TensorFlow Lite
- Flutter
- Mobile Application Development
- Calorie Estimation
- Data Preparation and Annotation

## Key Learning Outcomes

This project provided hands-on experience in:

- Building an applied AI system from problem definition to prototype
- Preparing and annotating image datasets
- Training an object detection model
- Evaluating model behavior under different real-world scenarios
- Optimizing a deep learning model for mobile deployment
- Integrating AI model outputs into a mobile application
- Thinking about user experience and practical product usage

## Project Type

Undergraduate Graduation Thesis  
Department of Electronics Engineering  
Gebze Technical University  
2024

## Note
<img width="370" height="721" alt="image" src="https://github.com/user-attachments/assets/7437a8e3-d94e-4434-a886-0a33e8f2df51" />

<img width="302" height="572" alt="image" src="https://github.com/user-attachments/assets/f4c61655-3538-478f-8acc-aad2cb640ea7" />


This repository is intended as a portfolio-style summary of the project. The original thesis includes the full project explanation, dataset design, model selection, mobile integration details, experimental results, and conclusion.
