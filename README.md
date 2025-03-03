# Fine-tuning a Vision Transformer for Indian Food Classification 🍛📷
This project demonstrates fine-tuning a Vision Transformer (ViT) model for image classification on an Indian food dataset using Hugging Face Transformers. The dataset consists of 6269 Indian dishes, and the model is trained to classify them accurately.

### 📌 Key Features
- **Dataset:** Indian Food Images (loaded via ImageFolder from local storage or Hugging Face Hub)
- **Model:** `google/vit-base-patch16-224-in21k` (pretrained ViT fine-tuned for classification)
- **Preprocessing:** Applied data augmentation (random cropping, flipping, normalization) using torchvision.transforms
- **Training:** Leveraged Hugging Face Trainer API with Accuracy as the evaluation metric
- **Fine-tuning:** Added a classification head to ViT and trained on the dataset
- **Evaluation:** Model tested and evaluated using the Hugging Face pipeline API
- **Deployment:** Model pushed to Hugging Face Hub for easy access and inference

### 🚀 Workflow
- **Data Preparation:** Mounted Google Drive, extracted images, and loaded them with datasets.ImageFolder
- **Preprocessing:** Applied transformations (resize, normalize, augment) before feeding data into the model
- **Model Training and Evaluation:** Validated model performance using test data and Accuracy metric
  - Batch size - 8
  - epoch - 4
  - accuracy - 0.91
  
- **Inference:** Loaded trained model and predicted labels for new food images

### 🔥 Results
- The fine-tuned model successfully classified various Indian food items
- Achieved an accuracy of 91% on the test set
- Model is available on the Hugging Face Hub for easy inference
