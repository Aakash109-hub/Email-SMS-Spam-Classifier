# Email/SMS Spam Classifier

This project is an **Email/SMS Spam Classifier** built using machine learning techniques. It classifies text messages or emails as **spam** or **ham** (non-spam). The model is trained using a dataset of labeled messages and employs popular text-processing techniques such as **TF-IDF** (Term Frequency-Inverse Document Frequency) and a **Multinomial Naive Bayes** classifier.

![Screenshot 2024-11-08 000335](https://github.com/user-attachments/assets/1be6b6da-82d4-4532-a925-a9c7bbdae938)


## Features:
- **Text Preprocessing**: The model processes and cleans text by removing stop words, punctuation, and applying stemming.
- **Model**: It uses **Multinomial Naive Bayes** for text classification, a simple yet effective model for spam detection.
- **Web Interface**: A user-friendly web interface powered by **Streamlit** allows users to interact with the model and classify their messages.

## How It Works:
1. **Text Input**: The user enters a text (email or SMS) into the provided input field.
2. **Model Prediction**: The text is processed and passed through the trained classifier.
3. **Spam or Ham**: The model classifies the text as either **Spam** or **Ham** and displays the result on the interface.

## Project Setup:

### Prerequisites:
To run this project locally, you’ll need:
- Python 3.x
- **pip** or **conda** for package management

### Installation:

1. **Clone the repository** (if applicable):
   ```bash
   git clone https://github.com/Aakash109-hub/Email-SMS-Spam-Classifier.git
   cd Email-SMS-Spam-Classifier
   ```

2. **Install dependencies**:
   If using `pip`:
   ```bash
   pip install -r requirements.txt
   ```

   If using `conda`:
   ```bash
   conda create --name spam_classifier_env --file environment.yml
   conda activate spam_classifier_env
   ```

3. **Download NLTK Resources**:
   In your Python script, ensure the following NLTK resources are downloaded:
   ```python
   import nltk
   nltk.download('punkt')
   nltk.download('stopwords')
   ```

4. **Run the Web App**:
   Launch the Streamlit app using:
   ```bash
   streamlit run app.py
   ```

### Web App:
You can also use the live web application for the classifier at the following link:
https://email-sms-spam-classifier-ak109.onrender.com

## Model Details:
- **Text Vectorization**: The input text is vectorized using **TF-IDF** to convert the text into numerical form suitable for machine learning.
- **Model**: The classifier used is **Multinomial Naive Bayes**, which is well-suited for text classification tasks like spam detection.


This project provides a simple and efficient way to classify email and SMS messages as spam or ham using machine learning. The interactive web interface allows users to easily classify their own messages.
