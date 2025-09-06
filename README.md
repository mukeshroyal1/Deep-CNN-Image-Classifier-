# Image Classifier - Happy/Sad Emotion Detection

A machine learning project that classifies images into "Happy" or "Sad" emotions using a trained neural network model.

## Project Structure

```
Image Classifier/
├── data/
│   ├── Happy/          # Happy emotion training images
│   └── Sad/            # Sad emotion training images
├── models/
│   └── happysadmodel.h5 # Trained model file
├── logs/               # Training logs
├── happyperson.jpeg    # Sample test image (happy)
├── nothappy.jpeg       # Sample test image (sad)
└── README.md
```

## Features

- **Binary Classification**: Distinguishes between happy and sad emotions in images
- **Pre-trained Model**: Includes a trained Keras model ready for inference
- **Dataset**: Contains 148+ labeled images for training and validation
- **Sample Images**: Includes test images for demonstration

## Model Details

- **Architecture**: Convolutional Neural Network (CNN)
- **Input**: Images (resized to standard dimensions)
- **Output**: Binary classification (Happy/Sad)
- **Format**: Keras H5 model file
  
## Training Loss and Accuracy 

<img width="547" height="461" alt="image" src="https://github.com/user-attachments/assets/540afedd-2ff6-4c1e-a30c-7f28565a6a8b" />

<img width="547" height="461" alt="image" src="https://github.com/user-attachments/assets/e86af6f4-8187-454c-a170-ad7662e26501" />


## Usage

The model can be loaded and used for emotion classification:

```python
import tensorflow as tf
from tensorflow.keras.models import load_model

# Load the trained model
model = load_model('models/happysadmodel.h5')

# Use the model for prediction
# (Implementation details would be in the Jupyter notebook)
```

## Dataset

- **Happy Images**: 81 images showing happy expressions and positive emotions
- **Sad Images**: 67 images showing sad expressions and negative emotions
- **Formats**: JPG, JPEG, PNG, WEBP
- **Quality**: Various resolutions and lighting conditions

## Requirements

- Python 3.x
- TensorFlow/Keras
- NumPy
- PIL/Pillow (for image processing)
- Matplotlib (for visualization)

## Note

This repository contains the trained model and dataset. The training code and implementation details are available in the Jupyter notebook (excluded from version control).

## License

This project is for educational and research purposes.
