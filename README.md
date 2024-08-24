# DNA Sequence Classification using Convolutional Neural Networks

This project uses a Convolutional Neural Network (CNN) to classify DNA sequences as promoters or non-promoters using the "Molecular Biology (Promoter Gene Sequences)" dataset from the UCI Machine Learning Repository.

## Requirements
- Python 3.7+
- TensorFlow 2.x
- NumPy
- Pandas
- Scikit-learn

## Installation
pip install tensorflow numpy pandas scikit-learn
## Usage
Run the main script: python dna_sequence_classifier.py

## Model Architecture
The CNN model consists of:
- Two 1D convolutional layers
- Two max pooling layers
- A flatten layer
- Two dense layers

## Data
This project uses the "Molecular Biology (Promoter Gene Sequences)" dataset from the UCI Machine Learning Repository. The dataset contains DNA sequences classified as either promoters or non-promoters.

Dataset URL: https://archive.ics.uci.edu/ml/machine-learning-databases/molecular-biology/promoter-gene-sequences/promoters.data

## Results
The model's performance can be evaluated using the printed test accuracy and sample prediction.

## Future Improvements
- Experiment with different model architectures
- Implement cross-validation
- Add data visualization for model performance
- Try other DNA sequence datasets
