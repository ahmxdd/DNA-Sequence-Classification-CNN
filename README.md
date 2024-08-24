# DNA Sequence Classification using Convolutional Neural Networks

This project uses a Convolutional Neural Network (CNN) to classify DNA sequences as promoters or non-promoters using the "Molecular Biology (Promoter Gene Sequences)" dataset from the UCI Machine Learning Repository.

## Packages and Language Used
- Python 3.7+
- TensorFlow 2.x
- NumPy
- Pandas
- Scikit-learn
- Requests

## Installation
pip install tensorflow numpy pandas scikit-learn requests
## Usage
Run the main script: python dna_sequence_classifier.py

## Model Architecture
The CNN model consists of:
- Two 1D convolutional layers
- Two max pooling layers
- A flatten layer
- Two dense layers

## Data
This project uses the "Molecular Biology (Promoter Gene Sequences)" dataset from the UCI Machine Learning Repository. The dataset contains DNA sequences classified as either promoters or non-promoters. The sequences are 57 base pairs long, and each base is represented as A, C, G, or T.

Dataset URL: https://archive.ics.uci.edu/ml/machine-learning-databases/molecular-biology/promoter-gene-sequences/promoters.data

Note: The data preprocessing step includes removing any whitespace, converting sequences to uppercase, and padding sequences to ensure uniform length.
## Results
The model's performance can be evaluated using the printed test accuracy and sample prediction. See the "DNA Sequence Classification project.ipynb" file for more information.

![image](https://github.com/user-attachments/assets/101ed5b4-60c3-45f3-aa23-b9aba97742ec)


## Future Improvements
- Experiment with different model architectures
- Implement cross-validation
- Add data visualization for model performance
- Try other DNA sequence datasets
