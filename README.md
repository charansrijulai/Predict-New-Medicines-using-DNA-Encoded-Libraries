# Predict-New-Medicines-using-DNA-Encoded-Libraries
The objective of this capstone project is to enhance small molecule binding prediction by utilizing machine learning (ML) techniques to explore a vast chemical space for potential drug candidates. Traditional drug discovery methods involve synthesizing small molecules individually and testing their interactions with specific protein targets. Given the estimated 10^60 potential drug-like compounds and the FDA's approval of only around 2,000 novel molecular entities, a more efficient approach is crucial. This project utilizes the Big Encoded Library for Chemical Assessment (BELKA), which contains data on approximately 133 million small molecules tested for binding to three protein targets using DNA-encoded chemical library (DEL) technology. In this project, we will develop predictive models to estimate the binding affinity of unknown chemical compounds to specified protein targets. Our approach will leverage the provided training data, while also exploring alternative methods for predicting small molecule binding without relying solely on empirical binding data. This will allow us to integrate various techniques to improve the accuracy and robustness of our predictions.


The distribution of smiles that binds with different protein names (BRD4, HSA, sEH) are: 
- The distribution on the left represents the training and validation datasets
- The distribution on the right corresponds to the evaluation dataset
![combined_viz](https://github.com/user-attachments/assets/63a3630c-9c7c-4e60-bcdc-9b0f49ac0c89)


The BELKA dataset can be found here -> [BELKA Dataset](https://www.kaggle.com/competitions/leash-BELKA/data?select=train.csv)
