# 🎵 LastSimilarious Web - Setup Guide

## 🔑 API Keys Required

This extension requires your personal API keys to work with Last.fm and YouTube services. **Never share your keys with anyone!**

### Step 1: Create Last.fm Account (if you don't have one)

1. **Go to [Last.fm Join Page](https://www.last.fm/join)**
   ![Last.fm registration page](https://via.placeholder.com/600x400/0D1117/FFFFFF?text=Last.fm+Registration+Page)
   - Fill in your details (username, email, password)
   - Confirm your email address
   - **Tip:** You can use an existing Last.fm account if you have one

### Step 2: Create Last.fm API Application

2. **Go to [Last.fm API Application Create](https://www.last.fm/api/account/create)**
   - Log in with your Last.fm credentials
   - Fill the form with the following information:

   **Application name:** `LastSimilarious Web`  
   *Yes, everyone will enter the same name - this is perfectly fine! Each user creates their own application instance.*

   **Application description:** `Browser extension for streaming music based on similar tracks from Last.fm`

   **Application homepage:** `https://github.com/aseni-teso/lastsimilarious-web`

   **Callback URL:** `http://localhost` or leave empty

   **Terms of service:** Check the box to agree

   ![Last.fm API application form](https://via.placeholder.com/600x500/0D1117/FFFFFF?text=Application+Name%3A+LastSimilarious+Web%0AHomepage%3A+https%3A%2F%2Fgithub.com%2Faseni-teso%2Flastsimilarious-web)

3. **Save your API keys**
   After submitting, you'll see your **API Key** and **Shared Secret**:
   ```
   API Key: 0123456789abcdef0123456789abcdef
   Shared Secret: 0123456789abcdef0123456789abcdef
   ```
   **⚠️ Important:** Copy and save these immediately! They won't be shown again.

### Step 3: Configure the Extension

4. **Install the extension** (unpacked developer mode or from store)

5. **Open extension settings**
   - Click the extension icon in your browser
   - Select "Options" or "Settings"
   - Enter your API Key and Shared Secret in the respective fields
   - Click "Save"

6. **Optional: YouTube API Key** (for better search results)
   If you want more reliable YouTube search, create a YouTube Data API key:
   - Go to [Google Cloud Console](https://console.cloud.google.com/apis/credentials)
   - Create a new project or select existing
   - Enable "YouTube Data API v3"
   - Create "API Key" credentials
   - Copy the key and paste in extension settings (optional)

## ⚙️ How It Works

- **Your keys stay on your computer** - stored locally in browser storage
- **No tracking** - the extension doesn't send your keys to any server
- **Individual quotas** - each user has their own API limits (important for YouTube API)

## 🛠️ Troubleshooting

**"Invalid API Key" error?**
- Double-check you copied the entire key (no spaces)
- Ensure you're using the "API Key", not "Shared Secret" in the API Key field
- Wait a few minutes after creating the key - it might need activation time

**"Application not approved" warning?**
- New Last.fm applications show this warning for 48 hours
- The extension will still work during this period
- The warning will disappear automatically after approval

**Need help?**
- Open an issue on [GitHub](https://github.com/aseni-teso/lastsimilarious-web/issues)
- Check [Last.fm API documentation](https://www.last.fm/api)

## 🔒 Security Notes

- Never share screenshots containing your API keys
- If you accidentally expose your keys, regenerate them in Last.fm settings
- The extension only makes requests to official Last.fm and YouTube APIs
- All data processing happens locally in your browser

---

**Enjoy streaming music with LastSimilarious Web!** 🎶

*This project is licensed under GPLv3. You are free to use, modify, and distribute this software under the terms of the GNU General Public License v3.0.*
