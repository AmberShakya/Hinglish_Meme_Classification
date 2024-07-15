# Internet Hinglish_Meme_Classification


## Overview
This project aims to develop a robust classification system for internet memes utilizing multimodal learning techniques. By leveraging both textual and visual information inherent in memes, the system seeks to accurately categorize memes into predefined classes or themes. The dataset used is sourced from the Memotion 3.0 competition, part of the De-Factify 2 workshop held in AAAI-22.

## Dataset
The dataset consists of 10,000 memes, including a subset of Hinglish memes, and is divided into three subsets:
- **Training Set**: 7,000 memes
- **Validation Set**: 1,500 memes
- **Test Set**: 1,500 memes

Each subset includes three CSV files providing metadata such as image IDs, corresponding labels (humor, sarcasm, offensiveness, motivational content), overall sentiment, and OCR text extracted from the memes.

## Tasks
The project focuses on two primary tasks within the Memotion 3.0 competition:

1. **Task A - Sentiment Analysis**: Classify memes into positive, negative, or neutral categories based on the sentiment conveyed.
2. **Task B - Emotion Classification**: Identify emotional nuances within memes, including humor, sarcasm, offensiveness, and motivational content.

## Model Architecture
The classification process involves using separate models for text and image data, followed by a combined analysis:

### Text-Only Model (DistilBERTMulti)
- **Architecture**: A condensed iteration of BERT trained on a multilingual corpus of 104 languages.
- **Advantages**: Computational efficiency, multilingual proficiency, transfer learning facilitation, cross-lingual applications.

### Image-Only Model (VGG16)
- **Architecture**: A convolutional neural network with 16 layers (13 convolutional layers and 3 fully connected layers).
- **Advantages**: Simplicity, effectiveness, transfer learning capability, robustness.

### Multimodal Model (DistilBERTMulti + VGG16)
- **Architecture**: Combines the strengths of both DistilBERTMulti and VGG16 by integrating feature extraction from text and images.
- **Advantages**: Comprehensive feature extraction, synergistic fusion, transfer learning, robustness, and generalization.


## Results
- **Task A**: Sentiment analysis plots (loss vs epochs, accuracy vs epochs) for the text-only and image-only models.
- **Task B**: Emotion classification results using the multimodal model.

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any changes or enhancements.

---
