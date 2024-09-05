# Emotion Recognition with DistilBERT

### Overview

This project focuses on the fine-tuning of the DistilBERT model for the task of recognizing emotions from text. By leveraging the power of transformer-based models, high accuracy in classifying emotions has been achieved.

### Dataset

The dataset used for training and evaluation was the "Emotion" dataset available on the Hugging Face Hub. It contains text samples labeled with different emotions such as sadness, joy, love, anger, fear, and surprise.

### Model

The DistilBERT model, a smaller and faster variant of BERT, was chosen for fine-tuning due to its efficiency in handling text classification tasks. The model was fine-tuned using the following specifications:

- Model Checkpoint: distilbert-base-uncased
- Number of Labels: 6 (corresponding to the six emotions in the dataset)

### Training

The model was fine-tuned using the Hugging Face Trainer. The following training parameters were used:
- Batch Size: 64
- Learning Rate: 2e-5
- Number of Epochs: 2
- Evaluation Strategy: Epoch-wise evaluation was performed to monitor the model’s performance during training.

The fine-tuning process was carried out on a GPU to accelerate the training time.

### Evaluation

The model was evaluated on the test set, achieving the following results:
- Test Accuracy: 91.8%
- Test F1 Score: 91.7% (weighted)

### Conclusion

This project demonstrates the effectiveness of fine-tuning transformer models like DistilBERT for emotion recognition tasks. The fine-tuned model can be utilized in various applications requiring sentiment analysis and emotional understanding.
  
