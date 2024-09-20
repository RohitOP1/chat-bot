# Chat Bot AI/ML Project

This project involves the development of a chatbot using Artificial Intelligence (AI) and Machine Learning (ML) techniques. The chatbot is trained to understand user queries and respond appropriately based on predefined intents.

## File Structure
- `training.py`: This file contains the code for training the chatbot model.
- `chatbot.py`: This file contains the code for running the chatbot.

## Data Preparation
- The training data is stored in a JSON file named `intent.json`, which contains intents along with corresponding patterns and responses.
- The NLTK library is used for text processing tasks such as tokenization, lemmatization, and bag-of-words creation.

## Model Training (`training.py`)
1. **Data Loading**: The training data is loaded from the `intent.json` file.
2. **Data Preprocessing**: Patterns and responses from the intents are extracted and tokenized using NLTK.
3. **Word Lemmatization**: Words are lemmatized to reduce them to their base forms.
4. **Word Vectorization**: The bag-of-words technique is applied to convert words into numerical vectors.
5. **Model Architecture**: A Sequential neural network model is built using Keras. The model consists of dense layers with ReLU activation and dropout for regularization.
6. **Model Compilation**: The model is compiled using the Stochastic Gradient Descent (SGD) optimizer and categorical cross-entropy loss function.
7. **Model Training**: The model is trained on the preprocessed data for a specified number of epochs.

## Chatbot Implementation (`chatbot.py`)
1. **Model Loading**: The pre-trained chatbot model is loaded from the `chatbotmodel.h5` file.
2. **Data Loading**: The words and classes used during training are loaded from the pickle files.
3. **Input Processing**: User input is cleaned, tokenized, and converted into a bag-of-words representation.
4. **Intent Prediction**: The model predicts the intent of the user input based on the bag-of-words representation.
5. **Response Generation**: Based on the predicted intent, a response is selected randomly from the predefined responses associated with that intent.
6. **User Interaction**: The chatbot continuously interacts with the user, predicting intents and generating responses based on user input.

## Technologies Used
- Python
- Libraries: NLTK, TensorFlow, Keras, NumPy
- File Serialization: Pickle (for storing words and classes)

## Setup and Installation
1. Install the required Python libraries (NLTK, TensorFlow, Keras).
2. Download the training data (`intent.json`) and place it in the project directory.
3. Run `training.py` to train the chatbot model and generate necessary pickle files and the trained model file.
4. Run `chatbot.py` to start the chatbot interaction. Enter messages in the console to chat with the bot.



For any improvements or feedback, please feel free to contribute or reach out.

### Connect me:
[Linkedin](https://www.linkedin.com/in/nirdesh-devadiya-55b408209)