# 🤖 OSINT Bot

A powerful Telegram bot for performing **OSINT (Open Source Intelligence)** tasks like:

- 📱 Phone Number Lookup  
- 🌐 IP Address Tracing  
- 🚗 Vehicle Registration Info  
- 🏦 IFSC Bank Code Lookup  
- 📧 Email Analysis  
- 🔍 Username Availability Check  
- 🖼 Image Metadata (EXIF)  
- 🧾 OCR (Text from Images)

> ⚠️ Educational use only. Respect privacy laws and Telegram TOS.

---

## 🚀 Features

- Fast & lightweight (async-powered)
- Channel join verification system
- Logs search history to **MongoDB**
- Optional logging to a **Telegram logs channel**
- Clean inline UI with buttons

---

## ⚙️ Tech Stack

- **Python 3.11**
- `python-telegram-bot v20+`
- `pymongo` (MongoDB)
- `requests`, `bs4` for scraping
- `opencv-python`, `pytesseract`, `pillow` for image analysis

---

## 🧪 Setup Locally

### 1. Clone the repo
```bash
git clone https://github.com/kratik00/bakchodiontop.git
cd bakchodiontop
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Add Tesseract (for OCR)
**Linux/Termux:**
```bash
sudo apt install tesseract-ocr
```

### 4. Set your configuration

Update `osint.py`:

```python
BOT_TOKEN = "your_bot_token"
ADMIN_ID = your_user_id
MONGO_URI = "your_mongodb_uri"
LOG_CHANNEL_ID = -100xxxxxxxxxx  # optional
```

---

## 🐳 Docker Setup

### Build Image
```bash
docker build -t osintbot .
```

### Run Bot
```bash
docker run -it osintbot
```

---

## ☁️ Deploy on Koyeb/Railway

- Make sure repo contains:

```
Dockerfile
Procfile
requirements.txt
osint.py
```

- Connect GitHub to Koyeb/Railway
- Set run command: `python osint.py`
- Environment variables can be used optionally

---

## 🛠 Commands List

| Command         | Description                    |
|----------------|--------------------------------|
| `/start`       | Show main menu                 |
| `/number`      | Phone number lookup            |
| `/ip`          | IP geolocation info            |
| `/ifsc`        | IFSC bank code info            |
| `/vehicle`     | Vehicle number info            |
| `/email`       | Email verification             |
| `/scan`        | Username scan on websites      |
| `/user`        | Telegram user profile info     |

---

## 🧾 Legal & Disclaimer

This bot is for **educational and research purposes only**.  
Using it against any individual’s privacy without consent is **strictly prohibited**.  
We do **not** store or sell any personal data.

---

## 🧑‍💻 Developer

Made with ❤️ by **LUCIFER**

- Telegram: [CHANNEL](https://t.me/URS_LUCIFER)
- Contact: t.me/lp_lucifer
