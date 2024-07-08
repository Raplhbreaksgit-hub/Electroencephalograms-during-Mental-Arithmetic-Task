# Electroencephalograms-during-Mental-Arithmetic-Task
# Electroencephalograms-during-Mental-Arithmetic-Task-Performance
Overview
This task is centered around the analysis of EEG data to classify different cognitive states
using advanced deep learning techniques. The data is sourced from the Mental Arithmetic
Tasks Dataset available at PhysioNet (https://physionet.org/content/eegmat/1.0.0/). The
dataset is pre-cleaned and ready for use, allowing you to focus on model implementation
and evaluation. Please familiarize yourself with the dataset by reviewing the accompanying
research paper (https://www.mdpi.com/2306-5729/4/1/14).

# Data
The data files with EEG are provided in EDF (European Data Format) format. Each subject has 2 files:

with "_1" suffix -- the recording of the background EEG of a subject (before mental arithmetic task)
with "_2" suffix -- the recording of EEG during the mental arithmetic task.
The recording datetime information has been set to Jan 01 for all files.

In this experiment all subjects are divided into two groups:

Group "G" (24 subjects) performing good quality count (Mean number of operations per 4 minutes = 21, SD = 7.4).
Group "B" (12 subjects) performing bad quality count (Mean number of operations per 4 minutes = 7, SD = 3.6).
In subject-info.csv, the "Count quality" column indicates which subjects correspond to which group (0 - Group "B", 1 - Group "G"). Additionally, subject-info.csv provides basic information about each subject (gender, age, job, date of recording).

I have downloaded the zip file then extracted the dataset and loaded the dataset from my device to my device and then used mne package of python for information visualizing and performing operations through mne.

# Objectives
You are required to implement and evaluate multiple deep learning models (suggesting to
implement at least 2 models) using the Python library MNE. Your analysis should be
documented in a Jupyter Notebook, which will be submitted via a GitHub repository link.

# Steps to Achieve It
1. Load the EEG data
2. Power Spectral Density (PSD) Analysis:
a. Calculate the band-wise PSD for both states: rest (recording eeg dataset
before mental arithmetic task) and task (recording of EEG dataset during the
mental arithmetic task). Focus on the following frequency bands: Delta (1-4
Hz), Theta (4-8 Hz), Alpha (8-12 Hz), Beta (12-30 Hz), and Gamma (30-100
Hz).
b. Compare the PSDs of the two states and summarize your findings.
3. Deep learning classification:
a. Extract relevant features from the cleaned data
b. Implement binary classification using any two different deep learning
models. You may choose from following models:
i. EEGNet
ii. TSCeption
iii. ViT (Vision Transformer)
iv. ATCNet
v. VAE (Variational Autoencoder)
c. Train and validate the model using the provided dataset.
d. Evaluate the models using appropriate metrics (accuracy, precision, recall,
F1-score) and discuss the results.

Submission Guidelines
● Ensure that your Jupyter Notebook is well-organized and thoroughly commented
● Share your completed notebook by submitting the GitHub repository link
