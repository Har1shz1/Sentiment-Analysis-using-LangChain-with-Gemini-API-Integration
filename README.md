
# 🧠 Sentiment-Analysis-using-LangChain-with-Gemini-API-Integration

A web-based tool built with **LangChain**, **Gemini 1.5 Flash**, and **Gradio** to analyze user feedback and extract key insights such as sentiment, emotion, and a 1–5 rating. It also provides visual visualizations to better understand user perception and experience.

---

## 🚀 Features

- 📈 **Sentiment Classification**: POSITIVE, NEGATIVE, NEUTRAL, IRRELEVANT, HARMFUL, or SUGGESTIVE
- 😊 **Emotion Detection**: Happy, Angry, Sad, Confused, and more
- ⭐ **Rating Prediction**: Scale from 1 (worst) to 5 (best)
- 📊 **Visual Charts**: Pie chart of sentiments, bar chart of ratings
- 📝 Accepts both manual feedback entries and `.txt` file uploads
- ⚡ **Powered by Gemini 1.5 Flash** with LangChain and Gradio interface

---

## 🔧 Installation

Install all the required Python packages using:

```bash
pip install -q --upgrade langchain-google-genai google-generativeai python-dotenv matplotlib pandas gradio
```

---

## 🔐 Setup API Key

This application uses **Gemini 1.5 Flash** from Google’s Generative AI suite. To use it, you’ll need to get an API key from [Google AI Studio](https://makersuite.google.com/app/apikey).

### ✅ Set the key in the script:
Replace this line:
```python
GOOGLE_API_KEY = "YOUR_API_KEY_HERE"
```

Or use a `.env` file:
```
GOOGLE_API_KEY=your_api_key_here
```

---

## 💻 How to Use

1. Run the script.
2. Gradio UI will open in your browser.
3. Either:
   - Enter multiple feedback entries manually (one per line), or
   - Upload a `.txt` file with feedback entries.
4. Click **"🔍 Analyze Feedback"** to get:
   - A results table showing Sentiment, Emotion, and Rating.
   - Two visual charts for insights: Sentiment Pie Chart and Rating Frequency Bar Chart.

---

## 📂 Example Feedback Input

```
I love the intuitive design and clean UI!
Too many bugs, I can't get anything done.
It's okay, does the job, nothing extraordinary.
```

---

## 🧾 Sample Output Table

| Feedback                                     | Sentiment | Emotion | Rating |
|---------------------------------------------|-----------|---------|--------|
| I love the intuitive design and clean UI!   | POSITIVE  | Happy   | 5      |
| Too many bugs, I can't get anything done.   | NEGATIVE  | Angry   | 1      |
| It's okay, does the job, nothing special.   | NEUTRAL   | Neutral | 3      |

---

## 📊 Charts

- **Sentiment Distribution (Pie Chart)**
- **Rating Frequency (Bar Chart)**

These help visualize the general tone and experience of users based on feedback.

---

## 🤝 Contributing

Found a bug or want to contribute new features? PRs and issues are welcome! Let's make it better together.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
