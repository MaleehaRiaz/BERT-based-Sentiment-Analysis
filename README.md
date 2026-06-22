## Project Title: Sentiment Analysis Using BERT Model 

## Project Overview
This project implements a transformer-based sentiment analysis system using the IMDB movie review dataset. The primary objective is to investigate the effectiveness of the pre-trained BERT model for text sentiment classification through fine-tuning.
The project includes complete data preprocessing, model training, evaluation, visualization, and prediction. Additionally, a separate PyTorch implementation was developed to further understand the architecture and training workflow of BERT-based sentiment classifiers.

## Objective
* Develop a complete sentiment analysis pipeline using BERT.
* Perform text preprocessing and sentiment label encoding.
* Fine-tune a pre-trained BERT moDEL for sentiment classification.
* Evaluate model performance using standard classification metrics.
* Explore both TensorFlow and PyTorch implementations of transformer-based sentiment analysis.

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
* Train-test-splits

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
* Cnfsion Matrix
* Classification Report (Precision, Recall, F1-score)
Training and validation curves are also visualized to monitor learning behaviour.

## Prediction
The trained model is tested on unseen text reviews to predict sentiment classes. Example inputs positive and negative product reviews to demonstrate inference using the fine-tuned model.

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
* Transformer-based Natural Languge Processing
* BERT fine-tuning
* Text preprocessing
* Model training and evaluation
* Deep learning workflows in TensorFlow and PyTorch
* Performance visualization and error analysis

## Future Work
Future improvements include:
* Training the PyTorch implementation on the complete IMDB dataset.
* Comparing multiple transformer models (RoBERTs, DistilBERT, DeBERTa).
* Investigating robustness under noisy and adversarial text inputs.
* Applying explainability techniques to better understand model predictions.
