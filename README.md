# Fake-news-classification
## Overview
This repository features the fine-tuning process for a version of the DistilBert model, trained on a [fake news articles dataset](https://huggingface.co/datasets/GonzaloA/fake_news). The model achieves exceptional performance on the evaluation set:  
- Loss: 0.0403  
- Accuracy: 98.92%
- F1 Score: 98.92%

The implemented model can be found on [HuggingFace](https://huggingface.co/jaranohaal/distilbert-base-uncased-finetuned-fake-news)

## Training procedure
The following hyperparameters were used during training:

- learning_rate: 2e-05
- train_batch_size: 32
- eval_batch_size: 32
- seed: 42
- optimizer: Adam with betas=(0.9,0.999) and epsilon=1e-08
- lr_scheduler_type: linear
- num_epochs: 2

## Training results

| Training Loss | Epoch | Step | Validation Loss | Accuracy | F1     |
|:-------------:|:-----:|:----:|:---------------:|:--------:|:------:|
| 0.03          | 1.0   | 762  | 0.0364          | 0.9880   | 0.9881 |
| 0.0121        | 2.0   | 1524 | 0.0403          | 0.9892   | 0.9892 |
