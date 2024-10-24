## Polymer Property Prediction using Transfer Learning



This repository contains the code and models used for predicting the mechanical and thermal properties of linear polymers using transfer learning. The work is based on the paper titled "Prediction of Mechanical and Thermal Properties of Polymers using Transfer Learning".

The prediction of mechanical and thermal properties of polymers is a critical aspect of polymer development. This repository demonstrates the use of a transfer learning approach to predict multiple properties of linear polymers. The neural network model is initially trained to predict the heat capacity at constant pressure (Cₚ) of linear polymers using 124 data points. The pre-trained model is then transferred to predict four additional properties: specific heat capacity (Cᵥ), shear modulus, flexural stress strength at yield, and dynamic viscosity. These properties represent a diverse set of mechanical, thermal, and rheological characteristics. The results show high accuracy in predicting these properties using small datasets (13 to 18 samples). Additionally, the base model's performance was evaluated using five different loss functions, with the combined loss function demonstrating superior performance.

## Repository Structure

1. Cp_Prediction_Model.ipynb
This notebook contains the neural network model used to predict the heat capacity at constant pressure (Cₚ) of linear polymers. It also explores the impact of various loss functions on model performance, including individual and combined loss functions.

2. Transfer_Learning_Models.ipynb
This notebook demonstrates the transfer learning process. The pre-trained Cₚ prediction model is adapted to predict the following four additional polymer properties:
Specific heat capacity (Cᵥ)
Shear modulus
Flexural stress strength 
Dynamic viscosity

3.Data Files
Datasets used for training and validation are included in the data/ folder, with a detailed description of each file's contents.

## How to use
requirements.txt
A list of dependencies and libraries needed to run the notebooks.
README.md
This file. It provides a detailed description of the project, instructions on how to run the notebooks, and a summary of results.
