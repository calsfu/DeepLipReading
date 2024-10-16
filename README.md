# Deep Lip Reading

## Overview

For this project, we are utilizing 2 datasets (LRW and Grid) to create lip-reading models (both CNNs and a Transformer).  Please see our submitted report for additional details on the project.  This project also contains an App that performers the lip-reading (word-by-word) in real-time.

Brief description of each file: 
 - **EC523_Group_Project_LipNET_V2.ipynb**: The CNN implemented on the Grid dataset (same used for LipNET)
 - **Grid-Transformer+CNN.ipynb**: Combination CNN and Transformer implemented on the Grid dataset (only partially functioning; not central to our analysis)
 - **Grid-Transformer.ipynb**: Transformer implemented on the Grid dataset
 - **LRW_ResNet_TCN.ipynb**: ResNet-TCN Hybrid implemented on the Lip Reading in the Wild (LRW) dataset
 - **LRW_res_tcn.pth**: PyTorch state dictionary for ResNet-TCN Hybrid LRW model
 - **LRW_transformer.ipynb**: Transformer implemented on the LRW dataset (only partially functioning; not central to our analysis)
 - **LRW_transformer.pth**: Pytorch state dictionary for LRW transformer model
 - **EC523_Group_Project_LipNET.ipynb**: Old/original version of this notebook
 - **grid-requirements.txt**: Used to pip install package dependencies for Grid notebooks (if running locally)
 - **req.txt**: Package requirements for the LRW dataset


# App Instructions

To run the App:
- cd App
- python3 app.py

How to use: 
- Face camera
- Start saying words
- Wait for prediction 

<img width="264" alt="Screenshot 2024-05-03 at 11 17 44 PM 1" src="https://github.com/chris-krenz/ec523-lip-reading-project/assets/74789609/bd4d7c17-f51e-443a-beb1-6d070a8b85d2">


# LRW Instructions

- Download dataset from https://www.robots.ox.ac.uk/~vgg/data/lip_reading/lrw1.html
- Place data in folder called lipread_mp4
- Run pip install -r req.txt to download the required packages
- Run LRW_CNN.ipynb or LRW_transformer.ipynb


# Grid Instructions

Intended to be run with Google Colab...
- Download the s1.zip and alignments.zip datasets from https://zenodo.org/records/3625687
- Extract the 'alignments' and 's1' folders to a zip called 'data.zip' and save it to the root of your Google Drive
- Run the notebook
- (If running locally, can use `pip install -r grid-requirements.txt' to install dependencies)
