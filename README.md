# ChatLens - WhatsApp Chat Analyzer
**ChatLens** is a powerful, interactive web application built with **Streamlit** that analyzes your WhatsApp chat history and presents detailed insights into your conversation patterns, activity timelines, most used words, emoji usage, and more — all locally, with no data sent to servers.

---

## Features
- **Top statistics**: Total messages, words, media shared, and links
- **Timelines**: Monthly and daily chat activity
- **Activity map**: Heatmaps and bar charts for most active days and hours
- **User comparison**: See who contributes most to the conversation
- **Word cloud**: Most common words used
- **Emoji analysis**: Which emojis are used most often
- **Filter by user**: Analyze individual participants or overall stats

---

## Tech Stack
```
Python Streamlit Pandas Matplotlib Seaborn WordCloud urlextract Emoji Regex
```

---

## Setup & Execution
1. **Clone the repository**
```bash
git clone https://github.com/Arpit12890/ChatLens-Whatsapp-Chat-Analyzer.git
cd ChatLens-Whatsapp-Chat-Analyzer
```

2. **Create and activate virtual environment (optional but recommended)**
```bash
python -m venv venv
.env\Scripts\activate   # On Windows
```

3. **Install dependencies**
```bash
pip install -r requirements.txt
```
> If you don't have a `requirements.txt`, manually install:
```bash
pip install streamlit pandas matplotlib seaborn wordcloud urlextract emoji
```

4. **Run the application**
```bash
streamlit run app.py
```
Then visit `http://localhost:8501` in your browser.

---

## Project Structure
```
ChatLens/
├── app.py              # Main Streamlit app
├── helper.py           # Logic for analysis and plotting
├── preprocessor.py     # WhatsApp chat parsing and cleaning
├── stop_hinglish.txt   # Custom stopwords for word filtering
└── README.md           # Project documentation
```

---

## How to Use
1. Export a WhatsApp chat (`.txt` format) from your phone
2. Run the app with `streamlit run app.py`
3. Upload the exported `.txt` file via sidebar
4. Explore insights using interactive visualizations!

---

## Privacy First
All processing is done **locally** in your browser or system — **no data is stored or sent to any server**.

---

## Author
Made by [Arpit Gupta](https://github.com/Arpit12890)

---

## License
This project is licensed under the MIT License.
