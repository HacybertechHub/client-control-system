## 🛡️ Hacyber Globaltech | Client Order Portal
A high-conversion, "Cyber Elite" aesthetic landing page designed for secure automation provisioning and client lead capture. This portal integrates **Google Sheets** as a backend, **Telegram** for instant notifications, and **Multi-Channel Email** routing.
## 🚀 Features
 * **Encrypted Aesthetic:** High-end dark mode UI with neon accents and Lucide icon integration.
 * **Automation Backend:** Uses Google Apps Script to log orders directly to a spreadsheet—no database required.
 * **Instant Alerts:** Telegram Bot API integration for real-time order notifications.
 * **Lead Tracking:** Built-in support for Facebook and TikTok pixels.
 * **Resource Center:** Integrated PDF preview modal and downloadable deployment contact sheets.
 * **Secure:** Built-in "Honeypot" anti-spam field and client-side validation.
## 📂 File Structure
To ensure the portal works correctly, keep your files organized like this on your server:
```text
/root-directory
│
├── index.html        # The main portal code
├── logo.png          # Your company branding (500x200 recommended)
├── notification.mp3  # Audio triggered on successful submission
└── HACYBER_Deployment_Contact.pdf  # The sheet clients preview/download

```
## ⚙️ Setup & Configuration
### 1. Google Sheets Integration
 1. Open a Google Sheet and go to **Extensions > Apps Script**.
 2. Deploy the provided doPost(e) script as a **Web App**.
 3. Set access to **"Anyone"**.
 4. Copy the URL and paste it into the GOOGLE_SCRIPT_URL variable in index.html.
### 2. Telegram Notifications
 1. Message @BotFather on Telegram to create a bot and get your **Token**.
 2. Message @userinfobot to get your **Chat ID**.
 3. Update the TELEGRAM_BOT_TOKEN and TELEGRAM_CHAT_ID constants in the script section.
### 3. Tracking Pixels
Replace the following placeholders in the <head> section:
 * YOUR_FACEBOOK_PIXEL_ID
 * YOUR_TIKTOK_PIXEL_ID
## 🛠️ Usage
When a client submits the form:
 1. **Sound:** notification.mp3 plays.
 2. **Data:** A new row is added to your Google Sheet.
 3. **Alert:** You receive a formatted message on Telegram.
 4. **Email:** A pre-filled email draft opens for the client to "Confirm" their order to your three support addresses.
 5. **Modal:** A success modal appears with direct links to your WhatsApp and Telegram channels.
**© 2026 HACYBERGLOBALTECH™. All Rights Reserved.**
