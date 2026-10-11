# DL-GSLC-Cat-Dog-Classification-Pandya_Zannito
Deep Learning image classification experiments using ResNet18 and MobileNetV2

# Cat and Dog Breed Classification

## About the Project

This project is part of a Deep Learning assignment. The goal is to classify images of cats and dogs into 10 different breeds using CNN models.

The experiments compare different training strategies and model architectures using ResNet18 and MobileNetV2.

## Dataset

The dataset is based on the Oxford-IIIT Pet dataset, using these 10 classes:

- Abyssinian
- Bengal
- Birman
- Bombay
- British Shorthair
- Beagle
- Chihuahua
- Japanese Chin
- Pug
- Samoyed

The data is split into training, validation, and test sets with a ratio of 70:15:15.

## Experiments

| Experiment | Description |
|---|---|
| B1 | ResNet18 trained from scratch |
| B2 | ResNet18 with a frozen backbone |
| B3 | ResNet18 with partial fine-tuning |
| B4-A | ResNet18 with data augmentation |
| B4-B | ResNet18 without data augmentation |
| B5 | MobileNetV2 with a frozen backbone |

## Results

B3 achieved the highest test Macro F1-score of 0.9765, with a test accuracy of 97.65%.

The experiments show that transfer learning performs much better than training the model from scratch on this dataset.

Note: The B4-A result could not be independently verified because its saved training history and checkpoint were identical to B2.

## Repository Contents

- `main.ipynb` — Notebook containing the experiments.
- `requirements.txt` — Required Python libraries.
- `outputs/` — Training histories, evaluation results, and visualization files.

## How to Run

1. Install the required libraries from `requirements.txt`.
2. Download the Oxford-IIIT Pet dataset.
3. Update the dataset paths in the notebook.
4. Open and run `main.ipynb`.

## Tools

- Python
- PyTorch
- Torchvision
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
