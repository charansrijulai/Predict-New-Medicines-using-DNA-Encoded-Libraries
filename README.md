# Predict-New-Medicines-using-DNA-Encoded-Libraries
The objective of this capstone project is to enhance small molecule binding prediction by utilizing machine learning (ML) techniques to explore a vast chemical space for potential drug candidates. Traditional drug discovery methods involve synthesizing small molecules individually and testing their interactions with specific protein targets. Given the estimated 10^60 potential drug-like compounds and the FDA's approval of only around 2,000 novel molecular entities, a more efficient approach is crucial. This project utilizes the Big Encoded Library for Chemical Assessment (BELKA), which contains data on approximately 133 million small molecules tested for binding to three protein targets using DNA-encoded chemical library (DEL) technology. In this project, we will develop predictive models to estimate the binding affinity of unknown chemical compounds to specified protein targets. Our approach will leverage the provided training data, while also exploring alternative methods for predicting small molecule binding without relying solely on empirical binding data. This will allow us to integrate various techniques to improve the accuracy and robustness of our predictions.


The distribution of smiles that binds with different protein names (BRD4, HSA, sEH) are: 
![train_viz](https://github.com/user-attachments/assets/d3b48540-2be1-4190-8e41-8ead33a2300e)



The BELKA dataset can be found here -> [BELKA Dataset](https://www.kaggle.com/competitions/leash-BELKA/data?select=train.csv)

# Project Architecture

![workflow](https://github.com/user-attachments/assets/e69bb8e0-9461-415d-b8a8-d20720fd3ba2)

The workflow begins with loading raw Parquet files into Google Cloud Storage, followed by preprocessing tasks like deduplication, encoding (Morgan fingerprints, ECFP), and transforming data from long to wide formats. EDA is performed to generate molecular descriptors, compute a correlation matrix, and prepare features for model training.
Machine learning models (e.g., Logistic Regression, Random Forest, CatBoost, XGBoost) are trained, and the best-performing model is deployed via an artifact registry, served through FastAPI and Streamlit for user interaction.

