# ComputerVision_PeerReviewed_Project---Facial_Keypoints_Detection
Project 1: Facial Keypoints Detection
### Project Experience
This is the first computer vision project which allows me to apply deep learning computer vision architectures(using **Pytorch**) to build a facial keypoint detection system for
- tracking, 
- pose recognition,
- filters
- emotion recognition.
### Image Augmentation
Introduce generalization(randomness) to detect and learn structures.
### Transform Steps:
Only the following transformation techniques were chosen to avoid unnecessary impacts on keypoints.

- **Rescale** to 250 for width and height
- **RandomCrop** to 224
- **Normalize & Convert ToTensor**

### Architecture & Performance
BatchSize, Epochs, Loss & Optimization Functions(only using **CPU**)

- **BatchSize** : 10(notebook stopped working if used batchsize higher than 20)
- **Epochs**   : 8(lower epochs was chosen due to hardware capacity constraint)
- **Loss**     : SmoothL1Loss(significant loss reduction since earlier epochs)
- **Optimizer** : Adam 

A simple model with 4 **Conv2D** layers, **ReLU** Activation, **MaxPooling**+**BatchNorm** in every layer, and **Dropout** to prevent overfitting.

### Worklist
> The project is broken up into four Python notebooks; 
> only **Notebook 2, 3 and models.py** file are graded.

### Files in Order
- data_load.py; models.py;
- Notebook 1. Load and Visualize Data.ipynb
- Notebook 2. Define the Network Architecture.ipynb
- Notebook 3. Facial Keypoint Detection, Complete Pipeline.ipynb
- Notebook 4. Fun with Keypoints.ipynb

LICENSE: This project is licensed under the terms of the MIT license.
