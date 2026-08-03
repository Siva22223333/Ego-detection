# Ego Detection

A computer vision project that detects whether a person in an image belongs to the registered user ("EGO") or not ("NOT_EGO") using a TensorFlow Lite image classification model.

---

## Overview

Ego Detection is a binary image classification system built with Python and TensorFlow. The model is trained on two classes:

- **EGO** – Images of the registered user.
- **NOT_EGO** – Images of other individuals.

After training, the model can classify new images and determine whether they belong to the registered user.

This project demonstrates the complete machine learning workflow, including dataset preparation, model training, TensorFlow Lite conversion, and inference.

---

## Features

- Binary image classification
- TensorFlow Lite model for lightweight deployment
- Image prediction using a trained model
- Easy-to-understand project structure
- Custom dataset support
- Beginner-friendly implementation

---

## Project Structure

```
Ego-detection/
│
├── dataset/
│   ├── EGO/
│   └── NOT_EGO/
│
├── train_model.py
├── predict.py
├── model.tflite
├── labels.txt
├── requirements.txt
├── README.md
└── assets/
    └── demo.png
```

---

## Technologies Used

- Python 3.x
- TensorFlow
- TensorFlow Lite
- OpenCV
- NumPy
- Pillow

---

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/Siva22223333/Ego-detection.git
```

```bash
cd Ego-detection
```

### 2. Create a virtual environment (Recommended)

**Windows**

```bash
python -m venv venv
venv\Scripts\activate
```

**Linux / macOS**

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

## Dataset Preparation

Create the following folder structure:

```
dataset/
│
├── EGO/
│     image1.jpg
│     image2.jpg
│     ...
│
└── NOT_EGO/
      image1.jpg
      image2.jpg
      ...
```

### Recommendations

- Use at least **200–500 images** for each class.
- Include different lighting conditions.
- Include multiple face angles.
- Avoid blurry images.
- Maintain a balanced dataset.

---

## Training the Model

Run:

```bash
python train_model.py
```

The training script will:

- Load the dataset
- Train the CNN model
- Evaluate performance
- Convert the model to TensorFlow Lite
- Generate:

```
model.tflite
labels.txt
```

---

## Running Prediction

Predict an image using:

```bash
python predict.py
```

The program loads:

- model.tflite
- labels.txt

and predicts whether the image is:

```
EGO
```

or

```
NOT_EGO
```

along with the confidence score.

---

## Example Output

```
Prediction : EGO

Confidence : 98.74%
```

---

## Requirements

Install all required packages:

```
tensorflow
opencv-python
numpy
Pillow
```

Or simply run:

```bash
pip install -r requirements.txt
```

---

## Future Improvements

- Real-time webcam detection
- Face recognition instead of image classification
- Live confidence visualization
- Mobile application using TensorFlow Lite
- Model optimization for edge devices
- Support for multiple registered users

---

## Applications

- Personal identity verification
- Smart attendance systems
- Personalized device access
- AI-based user authentication
- Computer vision learning projects

---

## Author

**Siva Shanmugam**

- GitHub: https://github.com/Siva22223333

---

## License

This project is licensed under the MIT License.

---

## Acknowledgements

This project was developed for educational purposes to explore:

- Deep Learning
- Computer Vision
- TensorFlow Lite
- Image Classification
- Python-based Machine Learning
