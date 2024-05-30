# ECG Signal Classification Task

This repository contains the code and dataset for Project 2 of the Advanced Machine Learning course at ETH. The goal of this project is to classify ECG signals into different classes.

## Table of Contents
- [Introduction](#introduction)
- [Dataset Specifications](#dataset-specifications)
- [Feature Extraction](#feature-extraction)
- [Tools and Libraries](#tools-and-libraries)
- [Files Description](#files-description)

## Introduction

Electrocardiogram (ECG) signals are used to monitor heart activity and can be classified into different categories based on various features. In this project, we aim to classify ECG signals into four different classes.

## Dataset Specifications

The dataset contains ECG recordings divided into four classes:

- **Class 0**
- **Class 1**
- **Class 2**
- **Class 3**

### Data Profile

| Label   | Number of Recordings | Mean | SD  | Max  | Median | Min  |
|---------|----------------------|------|-----|------|-----|------|
| Class 0 | 3030                 | 29.8            | 9.4  | 59.5| 27.9 | 8.3    |
| Class 1 | 443                  | 29.7            | 11.8 | 58.5| 27.8 | 9.0    |
| Class 2 | 1474                 | 31.9            | 11.0 | 58.9| 28.0 | 8.6    |
| Class 3 | 170                  | 22.2            | 10.0 | 57.2| 24.9 | 9.3    |
| **Total** | **5117**             | **30.1**         | **10.3** | **59.5** | **27.9** | **8.3** |

## Feature Extraction

For ECG signal classification, we use manual feature extraction techniques to derive meaningful features from the raw ECG data. Some of the key features include:

- **RR Interval**
- **R Amplitude**
- **Q Amplitude**
- **QRS Duration**
- **Heart Rate Variability**
- **Frequency Domain Features**

## Tools and Libraries

We use the following Python library for ECG signal processing and feature extraction:

- **Biosppy**: A library for biosignal processing.
  ```python
  import biosppy.signals.ecg as ecg 
  ```

## Setup and run

Run the files in the following order :
- **process.ipynb** : Extracts features from the ECG signal.
- **features.ipynb** : Scale and performs feature selection.
- **model.ipynb** : Trains the model and outputs the result of applying the model on **X_test.csv** in a file **out.csv**.

The datasets are supposed to be in a folder public, too big to be included in the repository.
