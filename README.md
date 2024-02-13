# CarPlateDetection

## Overview
CarPlateDetection is a project focused on the detection of license plates in images using a fine-tuned YOLO (You Only Look Once) model. This project aims to provide a high-performance solution for license plate recognition tasks by leveraging a dataset specifically tailored for this purpose.

## Features
- High accuracy license plate detection
- Fast processing times suitable for real-time applications
- Easy to install and deploy

## Installation
This project relies on several dependencies, including PyTorch, torchvision, and ultralytics, among others. We recommend using a conda environment for easy setup.

### Setting Up the Environment
1. First, create a conda environment:
   ```bash
   conda create -n torch-gpu
   ```
2. Activate the newly created environment:
   ```bash
   conda activate torch-gpu
   ```
3. Install the required packages using conda and pip:
   ```bash
   conda install -c pytorch -c nvidia -c conda-forge pytorch torchvision pytorch-cuda=11.8 ultralytics
   pip install -r requirements.txt
   ```

## Usage
To obtain a result in the form of a video it is recommended to follow the steps below:
1. Extract information from the source video:
   ```bash
   python main.py
   ```
2. Add extra data for better visualization:
   ```bash
   python src/add_missing_data.py
   ```
3. Generate output video:
   ```bash
   python src/visualize.py
   ```

For more information or if you encounter any issues, please open an issue on this GitHub repository.
