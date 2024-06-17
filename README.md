# Brain Tumor Detection with YOLOv9
This repository contains a Jupyter Notebook that demonstrates the use of YOLOv9 (You Only Look Once version 9) for detecting brain tumors in medical images. YOLOv9 is a state-of-the-art object detection model, and this notebook provides a step-by-step guide to setting up and running the model for brain tumor detection.

# Table of Contents
  1. Before You Start
  2. Clone and Install
  3. Download Model Weights
  4. Detection with Pre-trained Model
  5. Authenticate and Download the Dataset
  6. Train Custom Model
  7. Examine Training Results
  8. Validate Custom Model
  9. Inference with Custom Model
# Before You Start
Ensure that you have access to a GPU for faster processing. You can verify GPU access using the nvidia-smi command. If needed, navigate to `Edit -> Notebook settings -> Hardware accelerator`, set it to `GPU`, and click `Save`.

`!nvidia-smi`

# Clone and Install
Clone the repository and install the necessary dependencies.

`import os`

`HOME = os.getcwd()`

`print(HOME)`

`!git clone https://github.com/your-repository-url.git`

`%cd your-repository`

`!pip install -r requirements.txt -q`

# Download Model Weights
Download the pre-trained model weights required for brain tumor detection.

`!wget -P {HOME}/weights -q https://your-model-weights-url/model.pt`

# Detection with Pre-trained Model
Use the pre-trained model to perform detection on the example data.

# Authenticate and Download the Dataset
Authenticate with your dataset provider (e.g., Roboflow) to download the dataset. Ensure the dataset is saved inside the `{HOME}/your-repository` directory for successful training.

`from roboflow import Roboflow`

`rf = Roboflow(api_key="YOUR_API_KEY")`

`project = rf.workspace("your-workspace").project("brain-tumor-dataset")`

`dataset = project.version(1).download("yolov9")  # Adjust according to your model`

# Train Custom Model
Instructions and commands for training the model on the downloaded dataset will be provided in the notebook.

# Examine Training Results
Analyze the results of your model training.

# Validate Custom Model
Validate the performance of your custom model on a test dataset.

# Inference with Custom Model
Run inference using the trained model and visualize the results. If you want to run inference using your own file as input, upload the image to the notebook and update the `SOURCE_IMAGE_PATH` variable with the path to your file.

By default, the results of each inference session are saved in `{HOME}/your-repository/runs/detect/`, in directories named `exp`, `exp2`, `exp3`, etc. You can override this behavior using the `--name parameter`.
