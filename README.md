# MovieReview-RNNAnalyzer

MovieReview-RNNAnalyzer is a sentiment analysis project that leverages a Simple Recurrent Neural Network (RNN) to classify movie reviews as positive or negative. The project is built using TensorFlow, Keras, and Streamlit for deployment.

## 📦 Project Structure

* `embedding.ipynb`: Implements word embedding using Keras' Embedding layer to convert text into dense vector representations.
* `simplernn.ipynb`: Develops a Simple RNN model to classify IMDB movie reviews based on sentiment.
* `prediction.ipynb`: Contains functions to load the trained model and make predictions on new text inputs.
* `main.py`: Streamlit-based app for interactive sentiment analysis using the trained RNN model.

## 🚀 Features

* Word embedding using Keras Embedding Layer.
* Simple RNN model to classify movie reviews.
* Streamlit web application for easy user interaction.
* Sentiment prediction (Positive/Negative) based on the review text.

## 🛠️ Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/MovieReview-RNNAnalyzer.git
   cd MovieReview-RNNAnalyzer
   ```

2. **Install dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

3. **Download the IMDB dataset:**

   * The dataset will be automatically downloaded when running the scripts.

## 💡 Usage

1. **Train the RNN Model:**

   * Open `simplernn.ipynb` and run all cells to train the model and save it as `simple_rnn_imdb.h5`.

2. **Test the Model:**

   * Open `prediction.ipynb` to test the model using predefined reviews or custom text inputs.

3. **Run the Streamlit App:**

   ```bash
   streamlit run main.py
   ```

   * Enter a movie review in the text area to classify it as Positive or Negative.

## 📂 Data Preprocessing

* Text data is tokenized using the IMDB dataset's word index.
* Reviews are padded to a maximum length of 500 tokens for consistency.

## 🔥 Model Architecture

* Embedding Layer: Converts text to dense vector representations.
* SimpleRNN Layer: Processes the sequential data.
* Dense Layer: Output layer with sigmoid activation for binary classification.

## ✅ Example

Input:

```
This movie was absolutely amazing with stunning visuals and a captivating plot.
```

Output:

```
Sentiment: Positive
Prediction Score: 0.87
```

## 📝 License

This project is licensed under the MIT License.

## 🤝 Contributions

Contributions, issues, and feature requests are welcome! Feel free to check out the [issues page](https://github.com/your-username/MovieReview-RNNAnalyzer/issues).
