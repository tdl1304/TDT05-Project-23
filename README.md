# Visual Transformer (ViT)

This project predicts whether a patient has pneumonia based on X-ray images. It uses a fine-tuned classification model with feature extractors from ResNet-50 and ViT.

- Dataset: [Chest X-ray Classification Dataset](https://huggingface.co/datasets/trpakov/chest-xray-classification)
- Fine-tuned ViT classification model: [Download here](https://drive.google.com/file/d/1NGWYIu-d9GkdCoQTsCEiN5r9AdS5RbAR/view?usp=share_link)
- Fine-tuned ResNet classification model: 

## Configuration

### Training ViT Classifier
- Batch size: 16
- Learning rate (LR): 2e-4
- Epochs: 6

### Training ResNet-50 Classifier
- Batch size: 32
- Learning rate (LR): 0.001
- Epochs: 2

## Results

Here are the evaluation results in JSON format:

```json
[
  {
    "vit_model_epoch2_eval": {
      "accuracy_overall": 0.9759656652360515,
      "accuracy_label0": 0.9907084785133565
    }
  },
  {
    "vit_model_epoch4_eval": {
      "accuracy_overall": 0.9759656652360515,
      "accuracy_label0": 0.9965156794425087
    }
  },
  {
    "vit_model_epoch6_eval": {
      "accuracy_overall": 0.9759656652360515,
      "accuracy_label0": 0.9965156794425087
    }
  },
  {
    "resnet_model_epoch2_eval": {
      "accuracy_overall": 0.9759656652360515,
      "accuracy_label0": 0.9907084785133565
    }
  },
  {
    "resnet_model_epoch4_eval": {
      "accuracy_overall": 0.9759656652360515,
      "accuracy_label0": 0.9907084785133565
    }
  },
  {
    "resnet_model_epoch6_eval": {
      "accuracy_overall": 0.9759656652360515,
      "accuracy_label0": 0.9907084785133565
    }
  }
]
