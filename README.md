
# 🤖 Gemini AI Streamlit App

A multi-functional AI-powered web app using **Google's Gemini API** and **Streamlit**.
This app demonstrates powerful capabilities of **LLMs**, including:

* 💬 ChatBot — Ask anything from Gemini-Pro
* 🖼️ Image Captioning — Auto-generate captions for your uploaded images
* 🔡 Text Embedding — Get semantic vector embeddings from input text
* ❓ Ask Me Anything — General Q\&A using Gemini-Pro

---

## 🚀 Demo Features

| Feature          | Description                                                    |
| ---------------- | -------------------------------------------------------------- |
| ChatBot          | Interact with Gemini-Pro in natural language                   |
| Image Captioning | Upload an image and get a smart caption from Gemini-Pro-Vision |
| Embed Text       | Convert text to embeddings using `embedding-001` model         |
| Ask Me Anything  | General Gemini Q\&A interface with a simple UI                 |

---

## 🧰 Tech Stack

* [Streamlit](https://streamlit.io/)
* [Google Generative AI](https://ai.google.dev/)
* [Pillow](https://pillow.readthedocs.io/)
* [streamlit-option-menu](https://github.com/victoryhb/streamlit-option-menu)

---

## 🔧 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/gemini-ai-app.git
cd gemini-ai-app
```

### 2. Create Virtual Environment (Optional but Recommended)

```bash
python -m venv venv
source venv/bin/activate   # On Windows: venv\\Scripts\\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Add API Key

Create a `config.json` file in the root directory:

```json
{
  "GOOGLE_API_KEY": "your_api_key_here"
}
```

Get your API key from: [https://makersuite.google.com/app/apikey](https://makersuite.google.com/app/apikey)

### 5. Run the App

```bash
streamlit run main.py
```

---

## 📁 Project Structure

```bash
.
├── main.py                # Main Streamlit app interface
├── gemini_utility.py      # Utility functions for model interaction
├── config.json            # Your API key (excluded from GitHub)
├── requirements.txt       # List of dependencies
```

---

## 🧠 How It Works

* `main.py` handles the UI and user interactions.
* `gemini_utility.py` contains functions that connect to Gemini Pro and Gemini Vision models.
* Embeddings are generated using Google’s official `embedding-001` model.
* Chat sessions are preserved using Streamlit’s `session_state`.

---

## 📌 Notes

* **Never upload your real API key to GitHub!**
  Use `.gitignore` to exclude `config.json`.

---

## 🙌 Acknowledgments

* Thanks to [Google AI](https://ai.google.dev/) for the Gemini API
* Built using [Streamlit](https://streamlit.io/)

---
