# Deep-PHURIE: Hurricane Intensity Estimation with Deep Learning

## Overview

Deep-PHURIE is a deep learning-based model for hurricane intensity estimation from infrared satellite imagery. It utilizes convolutional neural networks (CNNs) to predict hurricane intensity based on provided features.

## Dataset

The model is trained on the TCIR-ALL dataset from 2017. The dataset contains infrared and passive microwave (PMW) data, with corresponding hurricane intensity labels (Vmax).

## Anaconda Environment

Ensure you have Anaconda installed. Create and activate the conda environment using the provided environment.yml file:

```bash
conda env create -f anaconda_env.yml
conda activate cyclone_env
```

## Exploratory Data Analysis (EDA)

Explore the dataset to understand its structure and characteristics:

```bash
# Run EDA
python EDA&Preprocessing.ipynb
```

## Model Architecture

### AlexNet

The model architecture is based on AlexNet and consists of convolutional layers, max-pooling layers, batch normalization, and fully connected layers.

### DeepPHURIE Model

Additionally, a modified DeepPHURIE model is implemented for hurricane intensity prediction using a different architecture.

## Training

The models are trained using k-fold cross-validation, and training results are visualized using matplotlib.

```bash
# Train the models
python Model_Training.ipynb
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
