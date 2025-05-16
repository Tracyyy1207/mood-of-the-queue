# 💡 Mood of the Queue

A lightweight internal Streamlit tool for logging and visualizing the mood of a support ticket queue throughout the day.

---

## 💡 Features

- Emoji mood logger 😠 😕 😊 🎉
- Optional notes for context
- Google Sheets as real-time backend
- Bar chart visualization of today's mood trend

---

## 🚀 Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/Tracyyy1207/mood-of-the-queue.git
cd mood-of-the-queue
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Set up Google Sheets API

- Go to [Google Cloud Console](https://console.cloud.google.com/)
- Enable **Google Sheets API** and **Google Drive API**
- Create a **Service Account**, download the `service_account.json` key file
- Place `service_account.json` in the project root directory
- Share your Google Sheet with the service account email (Editor access)

### 4. Run the app locally

```bash
streamlit run mood_logger.py
```

This will open the app at [http://localhost:8501](http://localhost:8501)

---

## 📝 Usage

1. Select a mood from the dropdown
2. (Optionally) add a note about how things feel
3. Click “Submit Mood”
4. View the bar chart showing today’s mood summary

---

## 🗂 Sample Google Sheet

| timestamp           | mood | note                    |
|---------------------|------|-------------------------|
| 2025-05-16 10:25:00 | 😠   | Issues with Rx queue    |
| 2025-05-16 11:40:45 | 😊   | Quick resolutions!      |
| 2025-05-16 13:55:10 | 🎉   | Celebrating success!    |

---

## 🔐 Security

Make sure you do **not commit** `service_account.json`.  
It should be added to `.gitignore` like this:

```bash
# .gitignore
service_account.json
```

---

## 📄 License

MIT

