# MNIST Digit Classification with CNNs 🧠

A comprehensive deep learning project implementing Convolutional Neural Networks (CNNs) for handwritten digit recognition using the MNIST dataset. This project explores both custom implementations and state-of-the-art architectures to achieve high classification accuracy.

## 📋 Overview

This project implements and compares multiple CNN architectures for classifying handwritten digits from the MNIST dataset:
- **Custom Implementation**: A baseline CNN model with batch normalization and early stopping
- **Advanced Model**: A deeper architecture inspired by top Kaggle submissions (99.6% accuracy) with data augmentation and learning rate scheduling

## ✨ Features

- 🎯 Multiple CNN architectures with different complexity levels
- 📊 Confusion matrix visualization for model evaluation
- 🔄 Data augmentation techniques (rotation, zoom, shifting)
- 📉 Early stopping and learning rate scheduling
- 🧪 Batch normalization and dropout for regularization
- 📈 Training history visualization

## 🏗️ Model Architectures

### Custom Implementation
- Conv2D layer (64 filters, 3×3 kernel) + Batch Normalization + MaxPooling
- Conv2D layer (128 filters, 3×3 kernel) + Batch Normalization + MaxPooling
- Dense layer (64 units) + Dropout (0.5)
- Output layer (10 units, softmax)

### Advanced Model (Based on Kaggle Top 10)
- Multiple Conv2D blocks with increasing filter sizes (32 → 64 → 128)
- Batch normalization after each convolution
- Strategic dropout layers (0.4) for regularization
- No pooling layers to preserve feature information
- Data augmentation for improved generalization

## 🚀 Getting Started

### Prerequisites

```bash
python 3.x
tensorflow
numpy
scikit-learn
matplotlib
```

### Installation

1. Clone the repository:
```bash
git clone https://github.com/patrickjcraig/DL-HW4.git
cd DL-HW4
```

2. Install dependencies:
```bash
pip install tensorflow numpy scikit-learn matplotlib
```

### Usage

Open and run the Jupyter notebook:
```bash
jupyter notebook main.ipynb
```

The notebook contains:
1. Data loading and preprocessing
2. Model architecture definition
3. Training with callbacks
4. Evaluation and visualization
5. Comparison between implementations

## 📊 Results

The project includes:
- **Confusion matrices** for both training and test sets
- **Accuracy metrics** comparing different architectures
- **Analysis** of architectural differences and their impact on performance

Results visualization can be found in the `Figures/` directory.

## 📁 Project Structure

```
DL-HW4/
├── main.ipynb              # Main implementation notebook
├── Figures/                # Generated visualizations
│   └── arch-1_conf_matrix.png
├── MNIST_ORG/             # MNIST dataset directory
├── DL-HW4.docx            # Project documentation
├── hmw4.pdf               # Homework assignment details
├── LICENSE                # MIT License
└── README.md              # This file
```

## 🔍 Key Insights

The comparison between implementations reveals:
- **Data augmentation** significantly improves generalization
- **Preserving features** (no pooling) can enhance accuracy in certain cases
- **Learning rate scheduling** helps fine-tune convergence
- **Deeper architectures** with proper regularization achieve better results
- **Validation split strategy** impacts model performance

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- MNIST dataset provided by TensorFlow/Keras
- Advanced model architecture inspired by [Kaggle top performers](https://www.kaggle.com/code/paulbacher/mnist-99-6-accuracy-top-10-leaderboard/comments)
- TensorFlow and Keras teams for excellent deep learning frameworks

## 📧 Contact

Patrick Craig - [@patrickjcraig](https://github.com/patrickjcraig)

Project Link: [https://github.com/patrickjcraig/DL-HW4](https://github.com/patrickjcraig/DL-HW4)

