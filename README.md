# NLP and Text Mining on Stack Overflow Data
Developed by G1T3 for IS450 - Text Mining and Analytics in AY2023-24 Term 2.
Click on this link to view the datasets `https://drive.google.com/drive/folders/1VTxC9AcTgzhghZd0REzfHZF6KLZwE5PU?usp=sharing`

## Overview

## Getting started
### GitHub Repository

### Prerequisites
Ensure you have `Cisco Secure Client` or `ClearPass` setup.

#### GPU setup
To connect to the GPU, please follow these steps:
- Connect to the Cisco secure network "svmpun2.smu.edu.sg/SMUVPN"
- After successful connecting, open up your command prompt and key in the userid `ssh IS450G2@origami.smu.edu.sg` and password

For further instruction on how to run the GPU:
- GPU Cluster documentation can be located at https://violet.smu.edu.sg/origami

### Installation

### Usage
#### LDA Model
1. Download the file 'LDA Model.ipynb' and under the 'Cell' tab on Jupyter Notebook, select 'Run All'.
2. If you would like to view the topic visualisation, you may download the file named 'topic_viz.html' and open it via the download folder on your laptop.

#### PTM4Tag Model
To train the model:
1. SSH into the GPU server
2. Once in the notebook, click into "ptm4tag_jolene.ipynb".
3. Run all the rows. Currently, the number of rows to train is set to 1 for testing purposes.
4. The data rows are saved as tensors in data folder.
5. The model is saved in "./results/save_me/epoch-2-file-0".

To test the model:
1. SSH into the GPU server
2. Once in the notebook, click into "ptm4tag_test.ipynb".
3. Run all the rows. Currently, the number of rows to test is set to 1 for testing purposes.
4. The results are saved in "test_results" folder in "result.csv".

Folder structure:

![image](https://github.com/jiaxuanchin/is450-g1t3/assets/114128066/3b39f1c0-74c6-4fd3-b585-54c6a06f1654)


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
1. Download the file "Reranking_model_NN.ipynb" and upload it onto your google drive.
2. Open it via google colab and click on run all.
