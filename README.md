# Deep Learning-based Multi-Character CAPTCHA Recognition

A deep learning project built using PyTorch to recognize and decode 6-character alphanumeric CAPTCHA images. The model treats each character position in the CAPTCHA as a separate classification task and trains six ResNet152 models, one for each character.

---

## Features

- Trains on 6-character CAPTCHA images
- Uses ResNet152 as the base model for character recognition
- One model per character position for higher accuracy
- Reports per-character accuracy and full CAPTCHA accuracy
- Works with custom datasets (just follow the naming convention)

---


The label for each image is extracted from the filename (e.g., `img1_ab123x.png` → label: `ab123x`).

---

## Model Architecture

- Backbone: `ResNet152`
- Output: 36-class classification for each character (0-9, a-z)
- Final prediction: Combine 6 outputs from 6 models to form the full CAPTCHA

---

## Technologies Used
Python 

PyTorch 

NumPy

PIL

Matplotlib

---

## Dataset

you can get captcha images dataset from kaggle ( https://www.kaggle.com/datasets/johnbergmann/captcha-image-dataset )



