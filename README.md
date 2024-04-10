# NLP and Text Mining on Stack Overflow Data
Developed by G1T3 for IS450 - Text Mining and Analytics in AY2023-24 Term 2.

## Overview

## Getting started
### GitHub Repository

### Prerequisites
Ensure you have `Cisco Secure Client` or `ClearPass` setup.

#### GPU setup

### Installation

### Usage
#### LDA Model
#### PTM4Tag Model
#### OVR Classifier with LinearSVC
The code for this model can be found in the [ovr_classifier_linearSVC.ipynb](./ovr_classifier_linearSVC.ipynb).

OVR Classifier is used to predict the top 3 most relevant tags for each Stack Overflow post. It accepts an input of the Title, Description and Code, and gives an output of the top 3 tags. A quick and simple demo is provided at the bottom of the python notebook for a more interactive experience.

A trained version of the model, as well as the TF-IDF model have been saved in `solution3_model400.sav` and `solution3_tfidf_vectorizer400.sav` respectively. 

**To use the trained version of the model, please only start running the code from the `Evaluation` section onwards. We will need to use the GPU for this.**

Below is a step-by-step on how to run the code on the GPU:
1. SSH into the GPU server
2. Enter `mynotebook` into the terminal / Command Prompt
3. Enter your email when prompted
4. Enter `2` to use a GPU enabled notebook
5. Enter `2` to use the Notebook with PyTorch
6. Open a new terminal / Command Prompt window and run the SSH command given
7. Enter the URL in a browser and operate as a normal Jupyter notebook. Run the relevant python notebook to train and run the model.

#### KMeans 
#### k-Nearest Neighbours
#### Neural Network
