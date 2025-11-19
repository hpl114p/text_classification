# Text Classification using BERT (HuggingFace Transformers)

This project implements a text classification model using BERT and the Transformers library from HuggingFace.
The model is fine-tuned on the NTC-SCV dataset for Vietnamese short-text classification.

![image](https://github.com/hpl114p/text_classification/blob/main/images/inference.jpg)

Live demo (Click icon below to run in Colab):

<a href="https://drive.google.com/file/d/1TgEa3xFwvNVxeMUiUkpVXw82n_F-itEF/view?usp=sharing"><img src="https://storage.googleapis.com/protonx-cloud-storage/colab_favicon_256px.png" width=80> </a>

## Features
* Fine-tuning BERT-base for sequence classification
* Tokenization using BERT tokenizer
* Training pipeline with PyTorch
* Evaluation: accuracy, F1-score
* Easy to extend for other classification datasets
* GPU-supported training (Google Colab)

## Model Architecture
* The model uses BERT Encoder + Classification Head: BERT Encoder (from bert-base-uncased)
* [CLS] token embedding extraction
* Dropout layer
* Linear classification layer