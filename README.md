# Waste_Classification
Waste Classification with Computer Vision

This project uses a deep learning model to classify waste images into six categories: cardboard, glass, metal, paper, plastic, and trash. The goal is to support automated recycling systems and reduce human sorting mistakes, improving sustainability and waste-management efficiency.

The model is built using transfer learning with EfficientNet-B0 pretrained on ImageNet. This approach allows strong performance with a small dataset and limited compute. Data augmentation, early stopping, and class-weighted loss are used to improve generalization and handle class imbalance. The project also includes Grad-CAM heatmaps to visualize what the model focuses on during predictions, increasing transparency and trust.

The dataset follows the TrashNet structure and is split into train, validation, and test folders. Training is performed in Google Colab using PyTorch. Evaluation includes accuracy, precision/recall by class, a confusion matrix, and visual explanation results. The target performance is 90%+ accuracy with strong recall for similar objects such as paper vs cardboard and plastic vs trash.

This repository contains the training notebook, data folder structure, and documentation. To run the model, upload your dataset to /content/data/ in Colab and execute the main notebook. The final deliverables include the trained model, performance metrics, and a short demo showing prediction results and Grad-CAM overlays on sample images.
