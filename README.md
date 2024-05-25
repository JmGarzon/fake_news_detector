# Fake News Detector

## Overview

This project is part of the class "Mining of Massive Data Sets" at Universidad EAFIT. It aims to detect fake news using various machine learning models implemented in Apache Spark. The project includes scripts for data preprocessing, feature extraction, and model training and comparison.

## Authors

- Jose Garzón
- Alejandro Salazar
- Germán Patiño

## Project Structure

- **moldes/**: This folder stores all the trained and generated models to be loaded for inference.
- **Fake News - Model Comparison - Spark.ipynb**: This Jupyter Notebook builds the pipelines and trains the different models for fake news detection.
- **previous_attempts/**: This folder contains old scripts that are no longer used but kept for reference.

## Requirements

To properly run this project, you need to have Git Large File Storage (LFS) installed. This is required to download the models and datasets used in the project.

## Installation

1. **Clone the repository:**
   ```sh
   git clone https://github.com/JmGarzon/fake_news_detector.git
   cd fake_news_detector
   ```


2. **Pull the LFS files:**

    ```sh
    git lfs install
    git lfs pull
    ```
3. **Extract the '.zip' files of interest.**

## Usage

- **Run the Jupyter Notebook:**
    Open Fake News - Model Comparison - Spark.ipynb in Jupyter Notebook and execute the cells to build the pipelines and train the models.

- **Load Pre-trained Models:**
    The pre-trained models stored in the moldes/ folder can be loaded for inference as needed.