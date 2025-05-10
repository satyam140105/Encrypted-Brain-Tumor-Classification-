# Brain Tumor Classification with Encrypted MRI Images

This project implements a lightweight Convolutional Neural Network (CNN) to classify brain MRI scans into four categories — **glioma**, **meningioma**, **no tumor**, and **pituitary tumor** — using **privacy-preserving encrypted image data**.

## 🔒 Key Features

- 🔐 **Encrypted Data Pipeline**: Images are encrypted using **Fernet (symmetric encryption)** to simulate secure healthcare data environments.
- 🔄 **Custom Data Generator**: A memory-efficient `tf.keras.utils.Sequence`-based generator decrypts images on-the-fly during training.
- 🧠 **CNN Model**: Compact model built using **TensorFlow/Keras** optimized for low memory environments.
- 📊 **Model Evaluation**: Includes classification report, confusion matrix, training plots, and sample predictions.
- 💾 **Model Saving & Logging**: Trained model and actual vs predicted labels are saved for further analysis.

## 🧪 Dataset

MRI image dataset organized in folders by class:

/Training
/glioma
/meningioma
/notumor
/pituitary
/Testing
/glioma
/meningioma
/notumor
/pituitary

> Dataset must be stored in your Google Drive for access through Google Colab.

## 🛠️ Technologies Used

- **Deep Learning**: TensorFlow, Keras  
- **Image Processing**: PIL  
- **Data Encryption**: Python Cryptography (Fernet)  
- **Visualization**: Matplotlib, Seaborn  
- **Environment**: Google Colab, Google Drive  
- **Utilities**: NumPy, Pandas, scikit-learn

## 🚀 How to Run

1. Mount your Google Drive in Google Colab.
2. Place your dataset in `drive/MyDrive/mini_proj/Training` and `Testing`.
3. Run the notebook: `brain_tumor_classification_encrypted_cnn.ipynb`.
4. Evaluate the model and save results.

## 📈 Results

- Achieved test accuracy of **~96%** 
- Visualized model performance with:
  - Accuracy/Loss plots
  - Confusion Matrix
  - Sample prediction results

## 📦 Output

- `brain_tumor_classifier_light.h5`: Trained model file  
- `actual_vs_predicted_sample.csv`: Sample predictions (100 images)  
- Training and evaluation plots

## 📄 License

This project is for educational and research purposes only.

---


