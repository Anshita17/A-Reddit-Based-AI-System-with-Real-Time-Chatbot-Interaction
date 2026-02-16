# 🧠 Mental Health Sentiment Monitoring and Support  
## A Reddit-Based AI System with Real-Time Chatbot Interaction

---

## 📌 Project Overview

Mental health discussions are increasingly taking place on social media platforms like Reddit, where users openly share emotional struggles, stress, anxiety, and depressive thoughts.

This project presents an **AI-powered real-time monitoring system** that:

- 🔎 Extracts Reddit posts related to mental health  
- 🧹 Cleans and preprocesses text using NLP techniques  
- 📊 Performs sentiment analysis using VADER and Transformer models  
- 🚨 Detects emotionally distressed posts  
- 🤖 Redirects users to an empathetic AI chatbot  
- 💬 Provides supportive real-time interaction  

The chatbot is powered by **DialoGPT (Hugging Face Transformers)** and deployed using **Gradio on Hugging Face Spaces**.

🔗 **Live Chatbot:**  
https://huggingface.co/spaces/AnshitaPriyadarshini17/Mental_Health_Chatbot

---

## 🎯 Objectives

- Automate detection of negative mental health posts
- Provide scalable and immediate emotional support
- Reduce dependency on manual moderation
- Demonstrate real-world application of NLP in mental healthcare

---

## 🏗️ System Architecture

Reddit API (PRAW)  
⬇  
Data Extraction  
⬇  
Text Preprocessing (NLTK)  
⬇  
Sentiment Analysis (VADER / DistilBERT)  
⬇  
Negative Threshold Detection  
⬇  
Reddit Bot Trigger  
⬇  
DialoGPT Chatbot (Gradio Interface)  

---

## 🛠️ Technologies Used

### Programming
- Python 3.9+

### NLP & ML
- NLTK
- VADER Sentiment Analyzer
- Hugging Face Transformers
- DistilBERT
- DialoGPT
- PyTorch

### Data Handling
- Pandas
- JSON

### Visualization
- Matplotlib
- Seaborn

### Deployment
- Hugging Face Spaces
- Gradio
- PRAW (Reddit API Wrapper)
- Flask (for local chatbot interface)

---

# 💻 How to Use This Project (3 Ways)

---

## 🟢 OPTION 1 — Run Locally (Flask Chatbot)

This runs the lightweight keyword-detection chatbot locally.

1. Clone the repository:

```bash
git clone https://github.com/Anshita17/A-Reddit-Based-AI-System-with-Real-Time-Chatbot-Interaction.git
cd A-Reddit-Based-AI-System-with-Real-Time-Chatbot-Interaction
```

2. Create virtual environment:

#### macOS / Linux
```bash
python3 -m venv venv
source venv/bin/activate
```

#### Windows
```bash
python -m venv venv
venv\Scripts\activate
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Run the Flask app:

```bash
python app.py
```

Open in browser:

```
http://127.0.0.1:5000
```

The chatbot responds to keywords like "help", "sad", or "thank", and can redirect users to the Hugging Face chatbot for advanced support.

---

## 🔵 OPTION 2 — Run Reddit Data Extraction (`test_reddit.py`)

This script fetches posts from a subreddit to analyze mental health discussions.

1. Make sure your Reddit credentials are set in `test_reddit.py`:

```python
import praw

reddit = praw.Reddit(
     client_id="YOUR_CLIENT_ID",
     client_secret="YOUR_CLIENT_SECRET",
     user_agent="MentalHealthBot",
     username="YOUR_REDDIT_USERNAME",
     password="YOUR_REDDIT_PASSWORD"
)
```

2. Run the script:

```bash
python test_reddit.py
```

3. It will print the top posts from the subreddit:

```
Post title: I feel so alone
Post title: Depression has taken over my life
...
```

> You can modify the subreddit and number of posts to monitor.

---

## 🟣 OPTION 3 — Use the Advanced AI Chatbot (Hugging Face)

For a more intelligent and context-aware experience, the live chatbot is hosted on Hugging Face Spaces:

👉 [Mental Health Chatbot](https://huggingface.co/spaces/AnshitaPriyadarshini17/Mental_Health_Chatbot)

No installation required. Provides empathetic conversation, context awareness, and supportive dialogue.

---

# 🤖 Chatbot Features

- Emotion-aware responses  
- Supportive conversational style  
- Maintains dialogue context  
- Non-judgmental tone  
- Encourages help-seeking behavior  

### 💬 Example Response

When a user types:

"I need help"

The system replies:

> "You're not alone. Our chatbot is here to support you.  
> 👉 [Chat Now 💙](https://huggingface.co/spaces/AnshitaPriyadarshini17/Mental_Health_Chatbot)"


---

# 📊 Results

- 2,000+ Reddit posts analyzed
- 73% sentiment classification accuracy
- Effective identification of strong negative emotional signals
- Real-time redirection to chatbot support

---

# 📈 Visualizations

- Word Cloud of Reddit Posts
- Sentiment Distribution Graph
- Emotional Pattern Analysis

---

# ⚠️ Ethical Considerations

- No permanent storage of user data
- No medical diagnosis provided
- Encourages professional help when required
- Designed strictly for supportive assistance

---

# 🔮 Future Improvements

- Emotion classification beyond polarity
- Multilingual support
- Crisis severity detection
- Integration with teletherapy platforms
- Fine-tuned mental health transformer models

---

# 🧠 Research Contribution

This project bridges:

- Social Media Mining
- Sentiment Analysis
- Conversational AI
- Real-Time Mental Health Support

It demonstrates how NLP can transform unstructured emotional discussions into structured and actionable support systems.

---

# 📬 Contact

Anshita Priyadarshini Mekatotti  
anshita.m04@gmail.com

---

⭐ If you found this project useful, consider giving it a star!
