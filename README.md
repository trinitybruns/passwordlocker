# password Locker
A modern, tabbed, encrypted password manager built with Python &amp; Tkinter.

🗝️ Password Locker (GUI Version)

A modern, tabbed, encrypted password manager built in Python using Tkinter.
This app securely stores your credentials behind a master password and provides a clean desktop-style interface for managing, generating, and tracking password expiration.

⭐ Overview

Password Locker is a fully functional GUI desktop application that allows you to:

Store passwords securely with encryption

Lock/unlock your vault using a master password

Add new accounts with custom password requirements

Generate strong passwords automatically

Track expiration dates

View and copy saved passwords

See expiring or expired passwords

Use a clean, organized, resizable window with tabs

This project is perfect for learning Python, practicing GUI development, and showcasing on GitHub.

✨ Features
🧩 Multi-Tab GUI Interface

The app includes:

Passwords Tab — view your saved entries

Add New Tab — create new entries with custom rules

Expiring Soon Tab — see passwords that expire within 14 days

Built using Tkinter’s Notebook widget for a full desktop app feel.

🔐 Master Password Protection

On startup, the app:

Prompts you to create a master password (first run)

Requires the master password to unlock your vault (future runs)

Allows 3 incorrect attempts before closing

Your master password is never stored — only a secure verification token is kept.

🛡️ Vault Encryption

All passwords and settings are encrypted using:

PBKDF2-HMAC-SHA256 key derivation

Fernet symmetric encryption (32-byte keys)

Unique salts stored in vault_config.json

Nothing sensitive is ever stored in plain text.

🤖 Password Generator

Each entry supports custom password requirements:

Minimum length

Require uppercase

Require lowercase

Require digits

Require symbols

Custom allowed symbol set

The generator creates strong, random, compliant passwords instantly.

🗓️ Password Expiration Tracking

For each password you can choose:

No expiration

Expire after X months

Expire on a specific date

The app shows statuses:

Valid

Expiring soon (under 14 days)

Expired

And lists all expiring/expired entries in a separate tab.

👀 Password Viewing & Copying

From the Passwords tab:

Select an entry

View masked details

Click Show Password

Click Copy Password to clipboard

📦 Installation
1. Clone the repository
git clone https://github.com/yourusername/password-locker-gui.git
cd password-locker-gui


(Replace yourusername with your GitHub username.)

2. Install required packages
pip install -r requirements.txt

3. Run the application
python main.py

🖥️ App Preview (Optional Screenshots)

You can add screenshots here, for example:

Master Password prompt

Main window

Add New tab

Expiring Soon tab

🔧 Project Structure
password-locker-gui/
├── main.py               # Main GUI application
├── requirements.txt      # Dependencies (cryptography)
├── vault.dat             # Encrypted vault (auto-generated)
└── vault_config.json     # Encrypted master-check config (auto-generated)

🛡️ Security Disclaimer

This project is designed for:

Learning

Personal organization

Portfolio use

Although it uses strong encryption, it is not intended to replace commercial password managers for storing highly sensitive information such as:

Banking credentials

Crypto wallet keys

Corporate secrets

Use responsibly.

🚀 Future Enhancements

Potential upgrades:

Edit existing entries

Delete entries

Add categories/tags

Search bar

Export/import encrypted vault

Light/dark/cute theme support

Desktop notifications

Multiple vault files

Auto-backup options

🤝 Contributing

Pull requests and enhancements are welcome!

📄 License

MIT License — free for personal or commercial use.

💖 Built With

Python

Tkinter GUI

Cryptography

Love for practical, simple, secure tools
