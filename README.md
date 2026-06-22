## Project Title: Sentiment Analysis Using BERT (IMDB Dataset)

## Project Overview
This project implements a transformer-based sentiment analysis system using the IMDB movie review dataset. The main objective is to evaluate the effectiveness of the pre-trained BERT model text sentiment classification through fine-tuning.
The project includes complete data preprocessing, model training, evaluation, visualization, and prediction. Additionally, a separate PyTorch implementation was developed to further understand the architecture and training workflow of BERT-based sentiment classifiers.

## Objective
* Build a sentiment analysis pipeline using BERT.
* Perform text preprocessing and sentiment encoding.
* Fine-tune a pre-trained BERT model for classification.
* Evaluate model using standard metrics (accuracy, F1-score).
* Explore TensorFlow and PyTorch implementations.
  
## Dataset Description
* Dataset: IMDB Movie Reviews Dataset
* Source: Kaggle
* Input: Movie reviews text
* Target: Sentiment labels

The dataset is cleaned by:
* Removing URLs
* Removing special characters
* Converting text to lowercase
* Removing unnecessary white space

## Methodology
## Data Preparation:
* Dataset loading with Pandas
* Missing value removal
* Text preprocessing using regular expressions
* Sentiment label encoding
* Train-test split

## Tokenization
* BERT Tokenizer (bert-base-uncased)
* Maximum sequence length: 128 tokens

## Model Architecture (TensorFlow)
* Pre-trained BERT encoder
* CLS token representation
* Fully connected dense layer (128 neurons)
* Dropout (0.3)
* Softmax output layer

## Training Configuration
* Optimier: Adam
* Learning Rate: 2 x 10⁻⁵
* Loss Function: Sparse Categorical Crossentropy
* Batch Size: 16
* Epochs: 5

## Model Evaluation
The model performance is evaluated using:
* Training Accuracy
* Validation Accuracy
* Training Loss
* Validation Loss
* Confusion Matrix
* Classification Report (Precision, Recall, F1-score)
Training and validation curves are also visualized to monitor learning behaviour.

## Prediction
The trained model is tested on unseen text reviews to predict sentiment classes. Example inputs include positive and negative reviews to demonstrate inference using the fine-tuned model.

## Additional PyTorch Implementation:
A separate PyTorch implementation was developed to understand the complete workflow of BERT-based sentiment classification, including:
* Custom Dataset class
* DataLoader
* BERT encoder
* Custom classification head
* Training loop
* Validation loop
* Performance visualization
*  Sample inference
This implementation serves as a practical demonstration of building a transformer-based classifier in PyTorch.

## Technologies Used
* Python
* TensorFlow
* PyTorch
* Hugging Face Transformers
* Scikit-learn
* Pandas
* Numpy
* Matplotlib
* Seaborn

## Learning Outcomes
Through this project, I gained practical experience in:
* Transformer-based Natural Language Processing
* BERT fine-tuning
* Text preprocessing
* Model training and evaluation
* Deep learning workflows in TensorFlow and PyTorch
* Performance visualization and error analysis

## Future Work
Future improvements include:
* Training the PyTorch implementation on the complete IMDB dataset.
* Comparing multiple transformer models (RoBERTa, DistilBERT, DeBERTa).
* Investigating robustness under noisy and adversarial text inputs.
* Applying explainability techniques to better understand model predictions.
