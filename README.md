# Text-Emotion-Classification
A deep learning project that classifies the emotional tone of text data into categories such as happiness, sadness, anger, love, fear, and surprise. Built using TensorFlow/Keras and deployed with an interactive Gradio UI. Inspired by and adapted from an article on The Clever Programmer and implemented in a Kaggle notebook by `https://github.com/OyewoleRasheed`.

---

## 🚀 Overview

This repository provides:

* **Data loading**: Uses the Emotions Dataset from [Praveen Govi's Kaggle dataset](https://www.kaggle.com/datasets/praveengovi/emotions-dataset-for-nlp).
* **Text preprocessing**: Tokenizes and pads sequences using Keras' `Tokenizer` and `pad_sequences`.
* **Model training**: Trains a TensorFlow/Keras Sequential model with Embedding and Dense layers to predict one of six emotions.
* **Gradio UI**: An interactive app that allows users to input text and see real-time emotion classification results.

## 📖 References

* Tutorial: [Text Emotions Classification using Python](https://thecleverprogrammer.com/2023/02/06/text-emotions-classification-using-python/)
* Dataset: [Emotions Dataset for NLP (Praveen Govi)](https://www.kaggle.com/datasets/praveengovi/emotions-dataset-for-nlp)
* Kaggle implementation: [rawsheed91 / Text Emotion Classification](https://www.kaggle.com/code/rawsheed91/text-emotion-classification)

---

## 🛠️ Installation

```bash
git clone https://github.com/OyewoleRasheed/Text-Emotion-Classification.git
cd Text-Emotion-Classification
python3 -m venv venv  # optional
source venv/bin/activate  # Linux/macOS
pip install -r requirements.txt
```

---

## 📂 Project Structure

```
├── text-emotion-classification.ipynb  # Jupyter Notebook (main implementation)
├── app.py                             # Gradio UI script
├── README.md                          # Project documentation
```

---

## ⚙️ Usage

### 1. Run the Notebook

Train the model and save artifacts by running all cells in `text-emotion-classification.ipynb`. It will:

* Download the dataset
* Preprocess the text
* Train the Keras model
* Save the model as `models/emotion_model.h5`
* Save the tokenizer as `tokenizer/tokenizer.pickle`

### 2. Launch Gradio UI

```bash
python app.py
```

## 💻 Gradio Interface

The Gradio app loads the trained Keras model (`models/emotion_model.h5`) and the tokenizer (`tokenizer/tokenizer.pickle`).

Enter any text snippet, click **Submit**, and the model will predict one of these emotions:

* joy
* sadness
* anger
* love
* fear
* surprise

---

## 📊 Results

The model achieves strong performance across emotions. Example metrics (as observed in the notebook):

* Accuracy: \~95%
* Loss: low after training epochs

Training graphs and evaluation metrics are plotted within the notebook.

---

## 📚 Dependencies

* Python 3.7+
* pandas
* numpy
* tensorflow
* sklearn
* gradio
* matplotlib

Install them via:

```bash
pip install -r requirements.txt
```
---

## 📄 License

MIT License. See [LICENSE](LICENSE) for details.

---

## 👤 Author

* **Oyewole Rawsheed** - [GitHub](https://github.com/OyewoleRasheed)

Feel free to open issues or reach out for questions!
