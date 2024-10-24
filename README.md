## Polymer Property Prediction using Transfer Learning



This repository contains the code and models used for predicting the mechanical and thermal properties of linear polymers using transfer learning. The work is based on the paper titled "Prediction of Mechanical and Thermal Properties of Polymers using Transfer Learning".

The prediction of mechanical and thermal properties of polymers is a critical aspect of polymer development. This repository demonstrates the use of a transfer learning approach to predict multiple properties of linear polymers. The neural network model is initially trained to predict the heat capacity at constant pressure (Cₚ) of linear polymers using 124 data points. The pre-trained model is then transferred to predict four additional properties: specific heat capacity (Cᵥ), shear modulus, flexural stress, and dynamic viscosity. These properties represent a diverse set of mechanical, thermal, and rheological characteristics. The results show high accuracy in predicting these properties using small datasets (13 to 18 samples). Additionally, the base model's performance was evaluated using five different loss functions, with the combined loss function demonstrating superior performance.

## Repository Structure

1. **PCA_Analysis.ipynb:**

   
This notebook is dedicated to performing Principal Component Analysis (PCA) on the dataset. It includes visualization of the principal components (PC1 vs. PC2, PC1 vs. PC3, etc.), which helps to understand the variance in the data and dimensionality reduction. PCA is especially useful for analyzing the relationships between various polymer properties.


2. **Cp_Prediction_Model.ipynb:**
   
This notebook contains the neural network model used to predict the heat capacity at constant pressure (Cₚ) of linear polymers. It also explores the impact of various loss functions on model performance, including individual and combined loss functions.

3. **Transfer_Learning_Models.ipynb:**

   
This notebook demonstrates the transfer learning process. The pre-trained Cₚ prediction model is adapted to predict the following four additional polymer properties:
Specific heat capacity (Cᵥ)
Shear modulus
Flexural stress strength 
Dynamic viscosity

4. **Data Files:**

   
Datasets used for training and validation are included in the data/ folder, with a detailed description of each file's contents.


## How to use
- Clone the repository.
- Open and run Cp_Prediction_Model.ipynb to train the base neural network model on Cₚ data with different loss functions.
- Open Transfer_Learning_Models.ipynb to see the transfer learning process and predict the four additional polymer properties.

## Results

Our approach demonstrates that transfer learning is highly effective for predicting various polymer properties, even when using small datasets. The model achieved high accuracy in predicting Cᵥ, shear modulus, flexural stress strength at yield, and dynamic viscosity. Additionally, we found that using a combined loss function led to better overall model performance compared to using individual loss functions.
