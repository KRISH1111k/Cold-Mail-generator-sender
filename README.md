# Cold-Mail-generator-sender

A lightweight Python tool to generate personalized cold emails from templates and send them using Gmail SMTP. Designed for early-stage founders, marketers, or interns at firms like Caprae Capital needing rapid outreach with minimal effort.

---

## 🚀 Features

- ✅ Auto-generates cold email content using pre-defined templates
- 📬 Sends emails via Gmail SMTP
- 🧠 Basic personalization per recipient
- 📊 Reads recipient lists from CSV files
- 🕵️‍♂️ Supports stealth mode: dry-run (preview without sending)

---

## 📁 Project Structure

coldmail-generator/
├── app.py # Streamlit UI (optional)
├── main.py # Core logic to generate/send emails
├── utils.py # Helper functions (e.g., template rendering)
├── contacts.csv # Sample recipient list
├── templates/ # Email templates (Jinja2 or plain text)
├── requirements.txt # Python dependencies
├── .env # Gmail credentials (NOT included in Git)
└── README.md # This file

yaml
Copy
Edit

---

## 🔧 How to Use

### 🔹 Setup

```bash
git clone https://github.com/<your-username>/coldmail-generator.git
cd coldmail-generator
pip install -r requirements.txt
🔹 Add Gmail credentials
Create a .env file with the following:

ini
Copy
Edit
EMAIL_USER=your-email@gmail.com
EMAIL_PASS=your-app-password
🔐 Use Gmail App Passwords for secure sending.

🔹 Run the tool
bash
Copy
Edit
python main.py
Or use:

bash
Copy
Edit
streamlit run app.py
For the UI-based version (if using Streamlit).

📝 Sample contacts.csv
csv
Copy
Edit
name,email,company
Alice Johnson,alice@example.com,ABC Corp
Bob Smith,bob@example.com,XYZ Inc
⚠️ Disclaimer
This tool is for educational and ethical outreach purposes only. Always comply with anti-spam laws like CAN-SPAM and GDPR when using bulk email tools.

🧠 Inspired by
Caprae Capital AI Internship Challenge

Cold outreach in early-stage VC / M&A lead generation

📜 License
MIT

yaml
Copy
Edit

---

## ✅ 2. `requirements.txt` (Minimal + Reliable)

Based on what this project likely uses, here’s your file:

streamlit
python-dotenv
jinja2
pandas
smtplib
email-validator

pgsql
Copy
Edit

> Note: `smtplib` and `email` are part of the standard library, so no pip install needed — but keep them mentioned in README usage if you use them.

You can generate this dynamically (if you’ve run everything locally):

```bash
pip freeze > requirements.txt
