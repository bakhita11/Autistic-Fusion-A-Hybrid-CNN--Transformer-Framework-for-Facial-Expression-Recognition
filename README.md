# Autistic Fusion: A Hybrid CNN–Transformer Framework for Facial Expression Recognition in Autistic and Non-Autistic Individuals

README.md

This repository contains the implementation of an autism detection framework that integrates multiple feature representations using an attention-based fusion mechanism. The project explores how combining distinct feature sequences—such as facial features, embeddings, and syntactic/contextual signals—can improve classification accuracy for identifying autistic versus non-autistic samples.
Project Overview
Traditional single-feature models often fail to capture the complex cues involved in autism detection. To address this, we propose a feature-level attention fusion model that combines multiple feature streams into a unified, discriminative representation.
The framework includes:
- Extraction of individual feature sequences  
- Attention-based fusion of complementary feature representations  
- Classification using a deep neural architecture  
- Evaluation with confusion matrix, class-wise metrics, and ROC curves
Key Features
Attention-Based Fusion: Learns optimal weighting between feature sequences.  
High Accuracy: Improved performance over baseline models.  
Explainability: Supports visualizations such as feature maps and attention heatmaps.  
Modular Design: Easy to replace or add additional feature extractors.

FERAC Dataset Direct Link:

https://www.kaggle.com/datasets/rajasreechaiti/ferac-dataset

Dataset Structure
The dataset is organized into the following directories:

./data/
   Autistic/
       ─ imgA.jpg
       ─ imgB.jpg
 ...
   Non-Autistic/
       ─ imgX.jpg
       ─ imgY.jpg
    ...
Dataset counts:
Class        	Train	Val	Test
Autistic	    1268	50	150
Non-Autistic	1268	50	150
Total	        2536	100	300

Installation
Clone the repository:
git clone https://github.com/bakhita11/Autistic-Fusion-A-Hybrid-CNN--Transformer-Framework-for-Facial-Expression-Recognition/tree/main
cd autism-detection-fusion
Install dependencies:
pip install -r requirements.txt

Run the training script:
python train.py
Run evaluation:
python evaluate.py
Generate visualizations (confusion matrix, class-wise metrics):
python visualize_results.py

