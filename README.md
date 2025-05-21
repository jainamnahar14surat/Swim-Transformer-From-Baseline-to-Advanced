# Swim-Transformer: From Baseline to Advanced

Here we are experimenting with different versions of the **Swim Transformer**, a lightweight yet powerful vision transformer architecture. This repository includes:

-  Baseline Swim Transformer  
-  Swim Transformer + ResNet  
-  Swim Transformer + Inception-ResNet  

> **Recommended Platform:** All models are Colab-compatible. For best results, run on [Google Colab](https://colab.research.google.com/) with GPU/TPU acceleration enabled.


## Contents

### 1. Swim Transformer

The baseline architecture inspired by hierarchical vision transformers with local self-attention. It's lightweight and effective for a variety of image classification tasks.

### 2. Swim Transformer + ResNet

A hybrid model combining the **Swim Transformer** with a **ResNet backbone**, aiming to improve feature extraction at earlier stages while leveraging the transformer's strength in global reasoning.

### 3. Swim Transformer + Inception-ResNet

A deeper hybrid variant merging **Inception-ResNet v2** modules for multiscale feature extraction with Swim’s transformer layers. This model aims for both efficiency and high accuracy across scales.


##  Comparison Table

| Model Variant                        | Train Loss | Train Accuracy | Test Loss | Test Accuracy | Inference Time (s) |
|-------------------------------------|------------|-----------|------------------|----------------|----------------------|
| Swim Transformer (Baseline)         | 0.0106       | 99.54%       | 0.8778            | 90.54           | 0.0874               |
| Swim Transformer + ResNet           | 0.0204      | 99.98%       | 1.0073            | 88.78       | 0.0527               |
| Swim Transformer + Inception-ResNet| 0.0658       | 97.27%       | 0.2709            | 91.99%         | 0.1214 |

> ⚠️ *Note: Values shown above are from test runs on ImageNet-like datasets. You can fine-tune these architectures on your custom dataset.*


##  How to Run (on Colab)

1. Open the corresponding notebook in the `/notebooks` directory.
2. Enable GPU via **Runtime > Change runtime type > GPU**.
3. Install dependencies and follow notebook instructions.
4. Upload your dataset or use built-in sample loaders.



