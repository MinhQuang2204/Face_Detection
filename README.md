# Face Recognition Project

This project demonstrates a complete pipeline for face recognition using ONNX models for face detection and recognition, and an SVM classifier for identity classification.

## How to use:

### Buoc1/ - Extract Faces

- **File**: `get_face.py`
- **Description**: This script captures faces from a video stream or image and saves the aligned faces into the `images/` directory.
- **Usage**: Rename the folder and file to the name of the first person you want to recognize. Run the program and press 'S' to extract face data. At least 2 images per person are required (it is recommended to extract as many face images as possible for accurate prediction, ideally around 50 images). Repeat this process for the next individuals.
-
- ![image](https://github.com/user-attachments/assets/407b6b81-9874-40e2-9adb-76421a30a668)

- ### Buoc2/ - Training

- **File**: `training.py`
- **Description**: This script loads the images from the `images/` directory, extracts features using the face recognition model, and trains an SVM classifier. The trained model is saved as svc.pkl.
- **Usage**: Simply run the script, and it will generate an svc.pkl file in the model/ directory.

