# Printed Text OCR and Generation using CRNN and GANs

This project combines a CRNN-based Optical Character Recognition (OCR) system with a baseline GAN model for generating synthetic printed text word images. The primary goal is to recognize and augment printed historical word-level text data, especially for ancient Spanish manuscripts.

## 🚀 Features

### ✅ CRNN-based OCR
- **Character Recognition using CRNN** (Convolutional Recurrent Neural Network)
- Achieved **99.5% accuracy** with **Greedy Decoding**
- Implemented **Beam Search Decoding** for sequence-level prediction
- Supports evaluation using **CER**, **WER**, and accuracy metrics
- Includes **Weighted CRNN** to handle class imbalance in character distribution

### 🎨 GAN-based Image Generation
- Baseline **DCGAN architecture** for generating printed word images
- Trained on limited dataset of real printed word images
- Generated images demonstrate potential but are visually noisy due to dataset constraints
- Plan to **fine-tune** GAN model and enhance output clarity

## 📊 Results

| Model           | Decoder            | CER    | Char Acc | WER    | Word Acc |
|----------------|--------------------|--------|----------|--------|----------|
| CRNN            | Greedy Decoding     | 0.0025 | 99.51%   | 0.0049 | 99.52%   |
| Weighted CRNN   | Greedy Decoding     | 0.0097 | 98.29%   | 0.0169 | 98.33%   |
| Weighted CRNN   | Beam Search Decoding| 0.0275 | 94.38%   | 0.0546 | 94.46%   |

## 🛠️ Technologies Used

- **Python**
- **TensorFlow / Keras**
- **NumPy / Pandas / Matplotlib**
- **CRNN Model** (CNN + BiLSTM + CTC Loss)
- **Beam Search Decoding**
- **DCGAN for Image Generation**
- **OpenCV** for preprocessing
- **Jupyter Notebooks** for training and evaluation


## 🔮 Future Work

- 🔧 Fine-tune the GAN model with more epochs and advanced loss functions
- 📈 Train GAN on a **larger and cleaner dataset** to improve image quality
- 🔄 Integrate GAN-generated samples into the CRNN training set for **data augmentation**
- 🧠 Explore **conditional GANs** to generate class-specific word images
- 🖋️ Expand model for **handwritten text** generation and recognition
- 🔍 Perform ablation studies on the effect of synthetic data on OCR performance
- 📂 Publish dataset and pretrained models for open research use

## 📬 Contact

For questions or collaborations, please reach out to **Naresh Meena** at - 
🔗 LinkedIn: [Naresh Meena](https://www.linkedin.com/in/nareshmeena12/).


