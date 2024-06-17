# Brain Tumor Detection with YOLOv9
This repository contains a Jupyter Notebook that demonstrates the use of YOLOv9 (You Only Look Once version 9) for detecting brain tumors in medical images. YOLOv9 is a state-of-the-art object detection model, and this notebook provides a step-by-step guide to setting up and running the model for brain tumor detection.

# Table of Contents
  1. Before You Start
  2. Clone and Install
  3. Download Model Weights
  4. Download Example Data
  5. Running the Model
# Before You Start
Ensure that your environment has access to a GPU for faster computation. You can verify GPU availability using the nvidia-smi command. If you encounter any issues, navigate to Edit -> Notebook settings -> Hardware accelerator, set it to GPU, and click Save.

To simplify managing datasets, images, and models, a HOME constant is defined to represent the current working directory.

# Clone and Install
YOLOv9 is very new and still under development. We recommend using a fork of the main repository due to a bug in the detect.py script that prevents inference. This bug is patched in the fork.

Clone the repository: Clone the YOLOv9 repository from the recommended fork.

Install the necessary requirements: Install all dependencies listed in the requirements.txt file from the cloned repository.

Install the roboflow package: This package is used to download datasets from Roboflow Universe.

# Download Model Weights
The YOLOv9 paper mentions several model versions (yolov9-s, yolov9-m), but the weights for these models are not yet available in the YOLOv9 repository. Download the available weights and save them to the weights directory.

# Download Example Data
To run inference using your own image file, upload the image to your environment and update the SOURCE_IMAGE_PATH with the path to your file. An example image can also be downloaded and used for testing.

# Running the Model
Follow the steps in the Jupyter Notebook to set up the environment, download the necessary weights and datasets, and run the model to detect brain tumors in medical images. The notebook provides detailed instructions and guidelines to guide you through the process.

This README file provides an overview of the notebook, setup instructions, and guidelines for running the YOLOv9 model for brain tumor detection. For detailed code and implementation, please refer to the provided Jupyter Notebook.
