# 🧠 Text Emotion Detection System

The **Text Emotion Detection System** is a machine learning-based web application that predicts the emotional tone behind a user's input text. It utilizes **Logistic Regression** with text vectorization techniques (CountVectorizer/TfidfVectorizer) to classify emotions and maps them to expressive **emojis**. The system includes a clean and interactive interface built with **Flask**.

---

## 🚀 Features

- Accepts any input text and predicts the emotion expressed
- Displays a matching **emoji** for better visual interpretation
- Shows the **confidence score** of the prediction
- Real-time predictions through a web-based interface
- Built-in text preprocessing (stopword removal, handle cleaning, etc.)
- Simple and intuitive **Flask UI**

---

## 🧰 Tech Stack

- **Python** for backend logic and model training
- **scikit-learn** for model training (Logistic Regression)
- **CountVectorizer / TfidfVectorizer** for text vectorization
- **NeatText** for text cleaning and preprocessing
- **Flask** for the web application
- **Altair** for optional visualizations
- **Jupyter Notebook** for model development and training

---

## 📊 Dataset

The model was trained using a labeled emotion dataset containing text-emotion pairs.  
Example entries:

Emotion Text

joy Sage Act upgrade on my to-do list for tomorrow.
sadness On the way to my homegirl's baby funeral!!!
surprise I got a gift! Hope you like it!


> The dataset includes 9 emotion labels: joy, sadness, anger, fear, surprise, neutral, disgust, shame, and happy.

---

## ⚙️ Installation Guide

Follow these steps to run the project locally:

### Step 1: Clone the Repository
git clone https://github.com/PhanindraSunkara/Text_Emotion_Detection.git
cd Text_Emotion_Detection

Step 2: Install Dependencies
pip install -r requirements.txt
Or manually:
pip install flask pandas numpy scikit-learn neattext altair

Step 3: Start the Web Application
python app.py

Open your browser at: http://127.0.0.1:5000



🧠 How It Works
1.The user inputs text into the web form.
2.The system cleans the text using NeatText (removing stopwords, handles, etc.).
3.The cleaned text is passed to the Logistic Regression model via a pipeline.
4.The predicted emotion is displayed with an appropriate emoji and confidence score.


🎭 Emoji Mapping

emotions_emoji_dict = {
    "anger": "😠", "disgust": "🤮", "fear": "😨😱", "happy": "🤗",
    "joy": "😂", "neutral": "😐", "sad": "😔", "sadness": "😔",
    "shame": "😳", "surprise": "😮"
}


✅ Results
Example Output:

📝 Input: "I can't believe I got the job!"
🎯 Predicted Emotion: joy
😊 Emoji: 😂
📊 Confidence: 0.86


🔮 Future Improvements
Enhancements that can be added to the project:

🚀 Use deep learning models like BERT for better accuracy
📈 Add graphical emotion probability distributions using Altair
🌐 Deploy on platforms like Heroku or Render
📱 Extend to a mobile app using Flutter or React Native
🗣️ Add speech-to-text input support

🤝 Contributing
Want to contribute? Awesome!

1.Fork this repository
2.Create your feature branch (git checkout -b feature-xyz)
3.Commit your changes
4.Push and open a pull request

Contributions, issues, and feature requests are welcome!
