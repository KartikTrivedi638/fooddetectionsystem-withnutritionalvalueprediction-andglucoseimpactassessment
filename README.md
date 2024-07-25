# fooddetectionsystem-withnutritionalvalueprediction-andglucoseimpactassessment
# Food Detection System with Nutritional Value and Glucose Impact Assessment

## Overview
A comprehensive tool for diabetic patients, this system uses a webcam to capture food images, predict their nutritional values with Inception V3, and estimate post-consumption glucose impact. Features an intuitive GUI for capturing, predicting, and displaying data.

## Features
- **Food Detection:** Utilizes the Inception V3 model, trained on 30 classes of food items, to accurately detect and classify food from webcam images.
- **Nutritional Value Assessment:** Provides detailed nutritional information for detected food items, sourced from an Excel database.
- **Glucose Impact Prediction:** Estimates the user's blood glucose level after food consumption based on selected pre-meal glucose levels.
- **User Interface:** Intuitive GUI with functionalities to capture images, predict food items, display nutritional values, select glucose ranges, and print post-consumption glucose levels.

## Model and Data
- **Model:** Inception V3, chosen for its high accuracy.
- **Training Data:** 6000 images
- **Validation Data:** 600 images
- **Test Data:** 960 images
- **Model Format:** .hdf5

## How It Works
1. **Capture Food Image:** Use the webcam to capture an image of the food item.
2. **Predict Food Item:** The model predicts the food item and provides a confidence score.
3. **Nutritional Information:** Retrieve and display the nutritional value of the detected food from an Excel file.
4. **Select Glucose Range:** Choose the current glucose range (80 to above 200) before eating.
5. **Predict Glucose Impact:** The system predicts and displays the estimated glucose level after consuming the food.

## Setup
1. Clone the repository and navigate to the project directory.
    ```sh
    git clone https://github.com/KartikTrivedi638/fooddetectionsystem-withnutritionalvalueprediction-andglucoseimpactassessment.git
    cd FoodDetectionSystem
    ```
2. Install the required dependencies from `requirements.txt`.
    ```sh
    pip install -r requirements.txt
    ```
3. Run the GUI script to start the application.
    ```sh
    python src/gui.py
    ```

## License
This project is licensed under the MIT License, a permissive open-source license that allows extensive freedom while ensuring proper credit to the original authors.
