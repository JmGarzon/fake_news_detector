# PENDIENTES: 
- Add G-drive link.
- Arreglar *etiquetas* del dataset y actualizar el script de preprocesamiento.
- Documentar el script de preprocesamiento. Configurar carpeta de entrada y salida en el repositorio.
- Añadir script de análisis, documentación en el readme y en el codigo.

# Fake News Detector

## Overview

This project is part of the class "Mining of Massive Data Sets" at Universidad EAFIT. It aims to detect fake news using various machine learning models implemented in Apache Spark. The project includes notebooks for data preprocessing, feature extraction, and model training and comparison.

## Authors

- Jose Garzón
- Alejandro Salazar
- Germán Patiño

## Project Structure

- **`logs/`**: Execution logs of the BERT + Classifier model.
- **`data/`**: This folder stores the data used to train the models.
- **`models/`**: This folder stores all the trained and generated models to be loaded for inference.
- **`notebooks/`**: This folder stores the Jupyter notebooks used to process the data, train and compare the models.

## Requirements
- Python libraries used can be installed using the `requierements.txt`.
- You need to have Git Large File Storage (LFS) installed. This is required to download the models and datasets used in the project.

## Models and Datasets:
* The contents of the `data/` and `models/` folders can be downloaded from: [LINK]

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

### Data preparation:
* Run `notebooks/Data_preproccesing.ipynb`, to read multiple CSV files in a `base_csv` folder containing news articles datasets. It processes them to standardize their schema, combines them into a single DataFrame, and saves the final DataFrame as a Parquet file. The steps include reading the data, standardizing the schemas, checking for duplicates, and saving the final processed data. The resulting parquet file should be placed inside `\data\news_data`.

### Models comparison:
*  Run `notebooks/Fake News - Model Comparison - Spark.ipynb` to train and compare a TFidF-based Logistic Regression,  a TFidF-based Random Forest, and a classifier using BERT embeddings.

## Usage of pre-trained models:
 * The pre-trained models stored in the `moldes/` folder can be loaded for inference as needed, in an independent inference pipeline.