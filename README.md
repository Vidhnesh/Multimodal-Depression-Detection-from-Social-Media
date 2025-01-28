# Multimodal-Depression-Detection-from-Social-Media
A machine learning project to detect depression from social media posts by combining text and image data. Used RoBERTa for text features, ResNet50 for image analysis, and EasyOCR for text extraction from images. Integrated metadata like emojis, hashtags, and engagement metrics, with multiple classifiers for robust detection.
**Features**
Text Analysis: Uses RoBERTa for extracting linguistic and semantic features.
Image Analysis: Utilizes ResNet50 for visual feature extraction.
Text from Images: Implements EasyOCR for extracting text embedded in images (e.g., quotes).
Metadata Integration: Includes emojis, hashtags, retweet, and like counts to enhance context.
Classification: Employs Logistic Regression, Random Forest, SVM, Neural Networks, and an ensemble method.

**Dataset Preparation**
Text Data Collection:
Collected ~6000 text records from Kaggle (Reddit posts related to depression).
Image Data Collection:
Included 2500 image-text records from social media platforms.
Used EasyOCR to extract text from images.
Metadata:
Added emojis, hashtags, retweet counts, and like counts to mimic real-world social media behavior.

**Data Preprocessing**
Text Preprocessing:
Tokenization and cleaning (removal of URLs, special characters).
Lowercased text and removed stop words for better feature extraction.
Image Preprocessing:
Resized images to 224x224 pixels.
Normalized pixel values for compatibility with ResNet50.

**Feature Extraction**
Text Features:
Used RoBERTa to generate embeddings from social media posts.
Image Features:
Employed ResNet50 for image pattern analysis.
Feature Fusion:
Combined text, image, and metadata features into a unified vector for classification.

**Model Training**
Classifiers Used:
Logistic Regression
Random Forest
Support Vector Machine (SVM)
Neural Networks (NN)
Ensemble Method (Voting Classifier)

**Evaluation Metrics:**
Confusion matrix, precision, recall, F1-score, and ROC-AUC were used to evaluate performance.
