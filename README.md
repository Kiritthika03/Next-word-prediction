# Next-word-prediction with LSTM
This project implements a Next Word Prediction web app using an LSTM (Long Short-Term Memory) neural network. The model was trained to predict the most likely next word based on an input sequence using deep learning and is deployed with a Streamlit interface.

✨ Features🔮 Predicts the next word from a given sequence of text
🤖 Uses a trained LSTM model (next_word_lstm.h5)
🧠 Tokenizer and sequence padding to handle real-time predictions
🌐 Simple and interactive UI using Streamlit
📂 Early stopping incorporated during training (not shown here but indicated)

📁 File Structure.
├── app.py                  # Streamlit application code
├── next_word_lstm.h5      # Trained LSTM model file
├── tokenizer.pickle       # Tokenizer used for input processing
└── README.md              # Project documentation🛠️ Installation & SetupClone the Repository
git clone https://github.com/yourusername/next-word-lstm.git
cd next-word-lstmInstall Dependencies
pip install -r requirements.txtYou may create requirements.txt with the following content:
streamlit
tensorflow
numpyRun the Streamlit App

streamlit run app.py📝 How It WorksThe user enters a partial sentence or a sequence of words.
The input is tokenized and padded to the required length.
The LSTM model predicts the most probable next word.
The predicted word is displayed in the Streamlit UI.
📸 UI PreviewAdd a screenshot here if available, e.g.:

📌 ExampleInput:to be or not to be
Output:Next word: [predicted_word]
🧠 Model Training (Summary)Although model training isn't shown here, it typically involves:
Preparing a text corpus
Tokenizing and creating n-gram sequences
Training an LSTM with sparse_categorical_crossentropy
Applying early stopping to prevent overfitting
