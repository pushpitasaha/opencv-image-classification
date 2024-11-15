# Waste Classifier Computer Vision Model

# Table of Contents

1. [Initial Setup](#initial-setup)
   - [Install Python 3.11](#install-python-311)
   - [Install VS Code 1.95](#install-vs-code-195)

2. [Object Detection Model Training](#object-detection-model-training)
   - [Categories](#categories)
   - [Train the model on Teachable Machine](#train-the-model-on-teachable-machine)

3. [Create Python Project in VS Code](#create-python-project-in-vs-code)
   - [Create a Folder](#create-a-folder)
   - [VS Code Setup](#vs-code-setup)
   - [Install Dependencies](#install-dependencies)
     - [Windows](#windows)
     - [macOS](#macos)
   - [Extract and Place Model](#extract-and-place-model)
   - [Run the Model](#run-the-model)
   
## Initial Setup
1. **Install Python 3.11**:  
   Download from [Python's website](https://www.python.org/downloads/release/python-3110/).

2. **Install VS Code 1.95**:  
   Download from [VS Code](https://code.visualstudio.com/download).

---

## Object Detection Model Training

1. **Categories**:
   - Paper Cups
   - Plastic Bottles
   - Metal Cans

2. **Train the model on Teachable Machine**:
   - Go to [Teachable Machine](https://teachablemachine.withgoogle.com/).
   - Choose "Image Project" > "Standard Image Model".
   - Name the three classes and capture training images.
   - Click "Train Model" and wait for the process to finish.
   - Export the model as **TensorFlow > Keras > OpenCV Keras**, then click "Download my model".

---

## Create Python Project in VS Code

1. **Create a Folder**:  
   Name it `object-detection`.

2. **VS Code Setup**:
   - Open VS Code and create a new file named `main.py`.
   - Copy the OpenCV Keras code snippet into the `main.py` file.

3. **Install Dependencies**:
   - Open a new terminal and follow these steps based on your OS:

   ### Windows:
   ```bash
   python -m venv .venv
   .venv\Scripts\activate
   pip install opencv-python tensorflow==2.15.1 keras==2.15.0 numpy
   ```

  ###MacOS:
   ```bash
    python3 -m venv .venv
    source .venv/bin/activate
    pip install opencv-python tensorflow==2.15.1 keras==2.15 numpy
   ```
4. **Extract and Place Model:**:

Extract converted_keras.zip from Teachable Machine and place the files in the object-detection folder.

5. **Run the Model:**

  In the terminal, run:
  ```bash
  python main.py
  ```
