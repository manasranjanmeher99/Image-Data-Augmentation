# 🚗 Image Data Augmentation & Image Classification using TensorFlow/Keras

## 📌 Project Overview

This project demonstrates two fundamental Computer Vision concepts using TensorFlow/Keras:

- 📸 **Image Data Augmentation**
- 🧠 **Image Classification using Pre-trained CNN Models (Transfer Learning)**

The notebook generates multiple augmented versions of an input image and classifies images using several popular pre-trained deep learning models trained on the ImageNet dataset.

---

# 📂 Project Structure

```
Image-Data-Augmentation/
│
├── data_argumentation.ipynb      # Main Jupyter Notebook
├── preview/                      # Generated augmented images
├── images/                       # Input image
│   ├── defender.webp
│   ├── dog.jpeg
│   └── peacock.jpeg
├── requirements.txt
├── README.md
```

---

# 🚀 Features

✅ Image Data Augmentation

- Rotation
- Width Shift
- Height Shift
- Shear
- Zoom
- Horizontal Flip
- Fill Missing Pixels

---

✅ Image Classification

The notebook performs image classification using the following pre-trained models:

- ResNet50
- ResNet50V2
- VGG16
- VGG19

All models are pre-trained on the **ImageNet** dataset containing over **1.2 million images** and **1000 object classes**.

---

# 🛠 Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- ImageDataGenerator
- ResNet50
- ResNet50V2
- VGG16
- VGG19

---

# 📦 Installation

Clone the repository

```bash
git clone https://github.com/manasranjanmeher99/image-data-augmentation.git
```

Move into the project folder

```bash
cd image-data-augmentation
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

# ▶️ Running the Notebook

Open Jupyter Notebook

```bash
jupyter notebook
```

Open

```
data_argumentation.ipynb
```

Run all cells.

---

# 📸 Image Data Augmentation

The notebook uses Keras' **ImageDataGenerator** to create new training images.

### Augmentation Parameters

```python
ImageDataGenerator(
    rotation_range=40,
    width_shift_range=0.2,
    height_shift_range=0.2,
    shear_range=0.2,
    zoom_range=0.2,
    horizontal_flip=True,
    fill_mode='nearest'
)
```

These transformations help improve model generalization and reduce overfitting.

---

# 📁 Preview Folder

The generated augmented images are automatically saved inside the **preview/** directory.

Example:

```
preview/
│
├── car_0_1234.jpeg
├── car_0_4567.jpeg
├── car_0_8912.jpeg
├── car_0_3456.jpeg
└── ...
```

These images are randomly transformed versions of the original input image and can be used to increase the size and diversity of your training dataset.

---

# 🧠 Image Classification

After augmentation, the notebook performs image classification using pre-trained CNN models.

The workflow is:

```
Input Image
      │
      ▼
Resize (224×224)
      │
      ▼
Preprocessing
      │
      ▼
Pre-trained CNN
      │
      ▼
Prediction
      │
      ▼
Top-3 Labels
```

---

# 📊 Models Used

| Model | Description |
|---------|------------|
| ResNet50 | 50-layer Residual Network |
| ResNet50V2 | Improved Residual Network |
| VGG16 | 16-layer Deep CNN |
| VGG19 | 19-layer Deep CNN |

---

# 📈 Sample Output

```
Predictions:

1. Jeep (0.92)
2. Pickup (0.05)
3. Sports Car (0.02)

Top Prediction Class Index: 609
```

---

# 🎯 Learning Outcomes

After completing this notebook, you will understand:

- Image preprocessing
- Data augmentation techniques
- Transfer Learning
- Pre-trained CNN models
- ImageNet dataset
- Image classification workflow
- Prediction decoding
- Comparing different CNN architectures

---

# 📸 Project Screenshots

## Original Image


(images/defender.webp)

---

## Augmented Images

```
preview/
```

Example:

preview/car_0_2088.jpeg
preview/car_0_2265.jpeg
preview/car_0_3534.jpeg

---


# 📚 Future Improvements

- Train a custom CNN model
- Fine-tune ResNet50
- Build a Streamlit web application
- Support batch image prediction
- Add real-time webcam classification

---

# 👨‍💻 Author

**Manas Ranjan Meher**

- GitHub: https://github.com/manasranjanmeher99
- LinkedIn: https://www.linkedin.com/in/manas-ranjan-meher-606985253/

---

## ⭐ If you found this project helpful, don't forget to star the repository!
