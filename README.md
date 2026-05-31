# Fruit Image Classification Using Deep Learning

This repository contains a multi-class fruit image classification project using deep learning. The project classifies fruit images into five categories:

- Apple
- Banana
- Grape
- Mango
- Strawberry

The work compares multiple deep learning approaches, including a custom CNN and transfer learning models, then identifies MobileNetV2 as the best-performing model.

## Project Summary

The project uses the Kaggle Fruits Classification dataset and follows a complete image classification workflow:

- Exploratory data analysis of the fruit image dataset
- Image cleaning and preprocessing
- Resizing images to 224 x 224 pixels
- Pixel normalization
- Data augmentation using flips, rotation, zoom, and contrast changes
- Training and comparing five model architectures
- Evaluation with accuracy, precision, recall, and F1-score
- Selection of the best model for deployment

## Models Compared

The project evaluates these models:

1. Simple custom CNN
2. MobileNetV2
3. ResNet50
4. EfficientNetB0
5. Xception

MobileNetV2 achieved the best overall result, with approximately:

- Accuracy: 87%
- Precision: 86.75%
- Recall: 87%
- F1-score: 0.867

## Repository Contents

```text
.
├── README.md
├── requirements.txt
├── original-files/
│   ├── Project2_Image_class.ipynb
│   ├── Multi-Class Fruit Image Classification Using Deep Learning.docx
│   └── Fruits-Classification.pptx
└── corrected-files/
    ├── Multi-Class Fruit Image Classification Using Deep Learning.docx
    └── Fruits-Classification.pptx
```

## File Notes

The original submitted files are preserved in `original-files/`.

While preparing the repository, the file extensions appeared to be mismatched:

- `Project2_Image_class.ipynb` appears to contain a Word document structure rather than a Jupyter notebook.
- `Multi-Class Fruit Image Classification Using Deep Learning.docx` appears to contain a PowerPoint presentation structure.
- `Fruits-Classification.pptx` appears to be the usable presentation file.

For convenience, corrected-name copies are included in `corrected-files/` where the internal file structure could be identified.

If you have the real Jupyter notebook source file, replace `original-files/Project2_Image_class.ipynb` with the valid notebook file before running the code.

## Dataset

Dataset used:

[Fruits Classification on Kaggle](https://www.kaggle.com/datasets/utkarshsaxenadn/fruits-classification)

Expected dataset structure:

```text
dataset/
├── train/
│   ├── Apple/
│   ├── Banana/
│   ├── Grape/
│   ├── Mango/
│   └── Strawberry/
├── valid/
└── test/
```

## Environment

The project was designed for:

- Python
- Jupyter Notebook
- TensorFlow/Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

Install the main dependencies with:

```bash
pip install -r requirements.txt
```

## How to Run

1. Download the dataset from Kaggle.
2. Place the dataset in the expected folder structure.
3. Open the Jupyter notebook.
4. Update dataset paths if needed.
5. Run the notebook cells from top to bottom.
6. Compare model performance and save the best model.

## Best Model

MobileNetV2 was selected as the best model because it provided the strongest balance between accuracy, F1-score, and training time. The model is lightweight and suitable for image classification tasks where inference speed matters.

## Future Improvements

- Re-export and include the valid Jupyter notebook source file.
- Fine-tune transfer learning backbones by unfreezing selected layers.
- Increase validation and test set size.
- Add a simple inference script for predicting fruit class from a new image.
- Deploy the model using Streamlit, Flask, or FastAPI.
