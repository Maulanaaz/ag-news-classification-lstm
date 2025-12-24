# 📰 AG News Classification using LSTM

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.20.0-orange)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📌 Project Overview

In this project, I utilize a **Recurrent Neural Network (RNN)** with **Long Short-Term Memory (LSTM)** architecture to solve the problem of multi-class news classification.

The model is trained on the AG News dataset to categorize news articles into four distinct topics: **World, Sports, Business, and Sci/Tech**. By leveraging LSTM, the model is designed to effectively capture sequential dependencies and semantic context within the text data, addressing the limitations of traditional models on unstructured data.

### 🎯 Project Goals

Based on the workflow implemented in the notebook, the main objectives of this project are:

1.  **Text Preprocessing:** Implement a cleaning pipeline (Regex removal, Lowercasing, Stopwords removal) to prepare raw text for modeling.
2.  **Sequence Processing:** Perform Tokenization and Padding to convert text into numerical sequences suitable for Deep Learning input.
3.  **Model Architecture:** Build and compile a Sequential LSTM network using TensorFlow/Keras.
4.  **Evaluation:** Analyze the model's performance using Accuracy and Loss metrics on unseen test data.

---

## 📂 Dataset

The project uses the benchmark **AG News Dataset**.
* **Source:** AG's Corpus of News Articles.
* **Classes:** 4 (Balanced).
    1.  🌍 World
    2.  ⚽ Sports
    3.  💼 Business
    4.  🚀 Sci/Tech
* **Input:** Title + Description of the news.
* **Output:** Class Label (0-3).

---

## 🏗️ Project Structure

The repository is organized to separate data processing, model definition, and training logic for reproducibility.

```text
├── notebook/              # Jupyter Notebooks (Original experimentation)
│   ├── notebook-ag-news-classification.ipynb
├── results/                # Evaluation metrics and plots
│   └── model_accuracy.png
│   ├── model_loss.png
├── requirements.txt        # Python dependencies
└── README.md               # Project documentation
```
## 🧠 Model Architecture

The model is built using TensorFlow/Keras with the following sequential layers:
1. Embedding Layer: Converts integer-encoded words into dense vectors to capture semantic meaning.
2. LSTM Layer: Processes the sequence information, retaining memory of previous inputs to understand context.
3. Dropout Layer: Randomly sets input units to 0 during training to prevent overfitting.
4. Dense Output Layer: A Softmax layer to output the probability distribution across the 4 classes.

## 📊 Results & Performance
After training the model, it achieved the following performance on the Test Set:
| Accuracy | Loss |
| :--- | :--- |
|87.1%                | 0.38 |

> (Note: The accuracy score above is based on the final evaluation on unseen test data.)

With the model accuracy plot :

![model_accuracy](https://github.com/Maulanaaz/ag-news-classification-lstm/blob/main/results/model_accuracy.png)

And model loss plot :

![model_accuracy](https://github.com/Maulanaaz/ag-news-classification-lstm/blob/main/results/model_loss.png)

## 📬 Contact
Created by **Maulana Zulfikar Aziz**
Connect with me on [LinkedIn](https://www.linkedin.com/in/maulanaaz)
