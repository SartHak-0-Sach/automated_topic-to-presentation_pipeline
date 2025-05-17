# 📽️ SlideGen – AI-Powered Slide Generator

Create stunning PowerPoint presentations 🎯 from simple topic prompts using **ChatGPT** + **DALL·E** + **Python-PPTX**. Whether you're working from a GUI, terminal, or a browser, SlideGen has you covered with three flavors:

* 🧠 GPT-driven content generation
* 🎨 AI-generated images per slide
* 🖼️ Clean and modern PPT export

---

## 📂 Project Structure

```
slidegen/
├── slidegen_airtable_pptx.py        # Airtable-powered script-based generation
├── slidegen_gui_tkinter.py          # Desktop GUI using Tkinter
├── slidegen_streamlit_app.py        # Web app using Streamlit
└── README.md                        # This documentation
```

---

## 🎯 Features

| Feature                       | Description                                                                |
| ----------------------------- | -------------------------------------------------------------------------- |
| 🧠 GPT-4 Powered Slides       | Generate intelligent slide content using OpenAI's Chat API                 |
| 🎨 DALL·E Slide Illustrations | Add an AI-generated image per slide for visual engagement                  |
| 🧾 PowerPoint Export          | Export final output in `.pptx` format using `python-pptx`                  |
| 🖥️ GUI + CLI + Web Modes     | Choose your preferred interface: terminal, desktop, or web                 |
| 📁 Batch Mode                 | Upload a `.txt` or `.csv` file with multiple topics for bulk deck creation |
| 📥 Download-Ready Decks       | One-click download buttons in GUI and Streamlit modes                      |
| 🧑‍💼 Airtable Integration    | Automate slide generation using Airtable records                           |
| 📋 Logging & Debugging        | Real-time logs and error messages                                          |

---

## 🚀 How to Use (Choose Your Flavor)

---

### 🖥️ 1. Desktop GUI (Tkinter) – `slidegen_gui_tkinter.py`

An easy-to-use interface for local desktop users.

#### ✅ Steps:

1. Run: `python slidegen_gui_tkinter.py`
2. Enter your topic (e.g., `Impact of AI on Healthcare`)
3. Click "Generate Slides"
4. Presentation saved as a `.pptx` in the same directory

✅ **Best for**: quick offline slide creation
📎 **Dependencies**: `openai`, `python-pptx`, `tkinter`, `Pillow`

---

### 🌐 2. Web App (Streamlit) – `slidegen_streamlit_app.py`

Interactive web interface that works in your browser.

#### ✅ Steps:

1. Run: `streamlit run slidegen_streamlit_app.py`
2. Choose:

   * Enter a topic
   * Upload `.csv` or `.txt` with multiple topics
3. Click **"Generate"**
4. Download your `.pptx` deck

🧠 DALL·E-generated images per slide are automatically embedded.

✅ **Best for**: teaching, live demos, bulk generation
📎 **Dependencies**: `openai`, `streamlit`, `python-pptx`, `Pillow`, `requests`

---

### 🔗 3. Airtable Automation – `slidegen_airtable_pptx.py`

Ideal for users managing topics via Airtable bases.

#### ✅ Steps:

1. Configure Airtable API key & Base/Table IDs
2. Run: `python slidegen_airtable_pptx.py`
3. Script fetches new records, generates decks, and updates Airtable with links/status

✅ **Best for**: workflows, automation, teams
📎 **Dependencies**: `openai`, `requests`, `python-pptx`, `pyairtable`

---

## ⚙️ Setup Instructions

### 1. 🔐 API Keys Required

Make sure to get your keys from:

* 🔑 [OpenAI API Key](https://platform.openai.com/account/api-keys)
* 🔑 Airtable API Key (if using Airtable mode)

You can set them as environment variables:

```bash
export OPENAI_API_KEY="your-openai-key"
export AIRTABLE_API_KEY="your-airtable-key"
```

Or directly in the script (not recommended for production).

---

### 2. 📦 Install Dependencies

All modules can be installed via pip:

```bash
pip install openai python-pptx streamlit pillow requests pyairtable
```

You may also use a `requirements.txt` file:

```bash
pip install -r requirements.txt
```

---

## 🧪 Demo Topics You Can Try

* “History of Machine Learning”
* “Benefits of Daily Exercise”
* “Solar Power: Past, Present & Future”
* “Climate Change and Policy Response”

---

## 🌍 Deployment Guide

### ▶️ Run Locally (GUI / Streamlit)

* For GUI:

  ```bash
  python slidegen_gui_tkinter.py
  ```

* For Streamlit:

  ```bash
  streamlit run slidegen_streamlit_app.py
  ```

---

### ☁️ Cloud Hosting (Optional)

#### 📡 Deploy on Streamlit Cloud:

1. Push this repo to GitHub
2. Go to [https://share.streamlit.io](https://share.streamlit.io)
3. Connect GitHub repo
4. Set environment variable: `OPENAI_API_KEY`
5. Click **Deploy**

---

## 💡 Customization Ideas

* ✨ Add themes or templates to your PPTs
* 🌐 Add multilingual support via GPT prompt tuning
* 🧵 Add narration using TTS libraries like gTTS or ElevenLabs
* 🧠 Add embeddings and search to reuse past topics
* 📨 Integrate with email for auto-sending decks

---

## 🐛 Troubleshooting

| Issue                     | Fix                                                                |
| ------------------------- | ------------------------------------------------------------------ |
| `OpenAI quota exceeded`   | Ensure billing is active or retry after cooldown                   |
| `Streamlit app crashes`   | Check for large file uploads or out-of-memory issues               |
| `No images in PPT`        | Ensure DALL·E prompt was successful; fallback to placeholder image |
| `Tkinter GUI not opening` | Ensure you’re not running in headless terminal (like WSL)          |

---

## 📜 License

This project is licensed under the **MIT License**.
Feel free to fork, remix, and build on it.

---

## 🙌 Contributors

Built by Sarthak Sachdev with love💘

---

## 📬 Feedback & Contact

Have suggestions or want to collaborate?

* Email: [Feel free to mail anytime](mailto:saarsaach30@gmail.com)
* portfolio website: [Checkout my other projects here](https://itsmesarthak.netlify.app/)

### Happy coding😇✨👍🏻
