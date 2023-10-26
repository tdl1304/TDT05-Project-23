# Visual Transformer (ViT)

This project predicts whether a patient has pneumonia based on X-ray images. It uses a fine-tuned classification model with feature extractors from ResNet-50 and ViT.

- Dataset: [Chest X-ray Classification Dataset](https://huggingface.co/datasets/trpakov/chest-xray-classification)
- Fine-tuned ViT/ResNet classification model: [Download here](https://drive.google.com/drive/folders/1VV4nW6UGPaTQdoGKZB3q2z1BRYF582hc?usp=drive_link)

## Configuration

### Training ViT Classifier
- Batch size: 32
- Learning rate (LR): 2e-4
- Epochs: 2

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
      "accuracy_overall": 0.9811
    }
  },
  {
    "resnet_model_epoch2_eval": {
      "accuracy_overall": 0.9785
    }
  }
]
```
