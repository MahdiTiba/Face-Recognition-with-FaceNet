# Face Recognition with FaceNet

This project focuses on performing face verification and recognition using FaceNet encodings.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Training](#training)
- [Evaluation](#evaluation)
- [Usage](#usage)
- [License](#license)

## Overview

Face recognition tasks are generally categorized into two types:

- **Face Verification**: Determines if a given image matches a specific identity (1:1 matching). Examples include unlocking a mobile phone using facial recognition.

- **Face Recognition**: Identifies the person in a given image from a database of known identities (1:K matching).

This project utilizes the FaceNet model to generate embeddings for facial images, which are then used for both verification and recognition tasks.

## Dataset

The dataset used in this project is located in the `datasets` directory. It contains images organized for training and evaluation purposes.

## Model Architecture

The project employs the FaceNet model, which maps facial images to a high-dimensional space where distances correspond to face similarity. The model architecture is defined in the `inception_blocks_v2.py` file, and utility functions are provided in the `fr_utils.py` file.

## Training

The training process involves the following steps:

1. **Data Preparation**: Loading and preprocessing images from the dataset.

2. **Model Compilation**: Configuring the FaceNet model with appropriate loss functions and optimizers.

3. **Model Training**: Training the model on the prepared dataset.

The training process is documented in the Jupyter Notebook `Face_Recognition.ipynb`.

## Evaluation

The trained model's performance is evaluated using various metrics to assess its accuracy in face verification and recognition tasks. Evaluation details are included in the `Face_Recognition.ipynb` notebook.

## Usage

To use the face recognition model:

1. Clone the repository:

   ```bash
   git clone https://github.com/MahdiTiba/Face-Recognition-with-FaceNet.git
   ```

2. Navigate to the project directory:

   ```bash
   cd Face-Recognition-with-FaceNet
   ```

3. Install the required dependencies.

4. Run the Jupyter Notebook:

   ```bash
   jupyter notebook Face_Recognition.ipynb
   ```

   This notebook contains code to load the trained model and perform face verification and recognition on new images.

## License

This project is licensed under the MIT License. For more details, refer to the `LICENSE` file in the repository.
