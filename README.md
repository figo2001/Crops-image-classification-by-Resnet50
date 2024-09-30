### Simplified Repository Structure

```
crops-classification-cnn/
│
├── data/
│   ├── train/           # Training data (folder for crops images)
│   ├── val/             # Validation data
│   └── test/            # Testing data
│
├── models/
│   └── CropModel.keras  # Saved Keras model
```

# Crops Classification using CNN

This repository contains code to classify crop images using a Convolutional Neural Network (CNN) built with TensorFlow/Keras.

## Requirements

To install the necessary packages, run:

```bash
pip install -r requirements.txt
```

## Data Preparation

1. Download the dataset and place it in the `data/` folder.
2. Organize the data into `train/`, `val/`, and `test/` directories, with subdirectories for each crop type.

## Training the Model

To train the model, run:

```bash
python train.py --epochs 20 --batch-size 32 --data-dir data/
```

## Making Predictions

To use the trained model for prediction, run:

```bash
python predict.py --image-path path/to/image.jpg --model-path models/cnn_crops_model.h5
```

```

### 2. **`requirements.txt`** (Dependencies)

```txt
tensorflow==2.6.0
numpy
pillow
scikit-learn
`` 
