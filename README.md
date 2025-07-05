# Image_classification_CNN
This project aims to build an image classification system using a Convolutional Neural Network (CNN) model with Transfer Learning, specifically leveraging the VGG16 architecture, to classify images into four custom categories: bike, cats, horses, and human.

The dataset used for this task is a manually created and organized folder-based image collection containing 975 images divided among the four classes. Each class has a varying number of samples, and all images are preprocessed to fit the input shape required by the VGG16 model (224x224 pixels).

Transfer Learning allows us to reuse the knowledge of a pre-trained model (VGG16 trained on ImageNet) and fine-tune it for our specific classification task. This significantly reduces training time and improves accuracy even with a smaller dataset.

The model achieved high accuracy (about 90%) after a few epochs of training, demonstrating the effectiveness of transfer learning in small custom datasets.
🔍 Objective:
i.To classify images into 4 categories: bike, cats, horses, and human.
ii.To implement a CNN using a pre-trained VGG16 model.
iii.To evaluate performance on a small dataset.
iv.To test predictions on new single images.

🛠 Technologies & Tools:
Python
PyTorch
Google Colab
Matplotlib / PIL for image display
VGG16 from torchvision.models

📂 Dataset Overview:
Total images: 975
Classes: bike, cats, horses, human
Format: Folder-based (used with ImageFolder)
Source: Custom (stored in Google Drive)
Preprocessing: Resized to 224x224, normalized

🔁 Process Workflow:
Data Loading: Using PyTorch's ImageFolder and DataLoader.
Preprocessing: Resize, normalization, and batch loading.
Model: Load pre-trained VGG16, freeze base layers, modify classifier.
Training: 5 epochs, CrossEntropyLoss, Adam optimizer.
Evaluation: Print accuracy and visualize predictions.
Testing: Predict and show results on individual images.
