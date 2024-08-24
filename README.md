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
- Dense layer with L2 regularization and ReLU activation
    - Dropout layer (50% dropout rate)
    - Outpit dense layer with softmax activation
 
### Model Training
- Data has training and testing sets
- Class weights are computed to handle class imbalance
- Model is trained for 50 epochs with a batch size 32.
- Training history (accuracy and loss) is plotted

### Evaluation and Prediction
- Model evaluated on test set
- Sample prediction is made to show the model's output

## Why use a CNN?
CNNs have been used a lot with identifying DNA sequences (Gunasekaran H, Ramalakshmi K, Rex Macedo Arokiaraj A, Deepa Kanmani S, Venkatesan C, Suresh Gnana Dhas C. Analysis of DNA Sequence Classification Using CNN and Hybrid Models. Comput Math Methods Med. 2021 Jul 15;2021:1835056. doi: 10.1155/2021/1835056. PMID: 34306171; PMCID: PMC8285202.)

Using a CNN in this scenario allows the model to learn complex features, from base pair patterns to more complex sequences.

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
