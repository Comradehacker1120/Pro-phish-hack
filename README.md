# Pro-phish-hack
CMDHCK Phish 🐟

CMDHCK Phish is a Python-based phishing tool for educational and security testing purposes, supporting 70+ website templates like Facebook, Instagram, and GitHub. 🚀 Use responsibly and only with permission!

Features ✨





📋 70+ phishing templates



🌐 Tunneling: Cloudflared, LocalXpose, LocalHostRun, Serveo



🎭 Custom URL masking



📧 Gmail credential capture (with app password)



🖥️ Supports Linux, Termux, macOS



🎨 Colorful interface with progress bars



🛠️ Custom site files and OTP pages



🔄 Auto-installs dependencies and updates

Requirements 📦

Software 🛠️





Python 3 🐍



PHP 💻



SSH 🔑



pip 📦

Python Modules 📚





requests, rich, beautifulsoup4 (as bs4)

Hardware/OS 💾





Linux 🐧, Termux 📱, or macOS 🍎



Internet connection 🌍



Termux: Enable storage and hotspot

Optional 🔧





LocalXpose account 🔗 (for auth token)



Gmail with app password 📧

Installation 🛠️





Clone Repository 📥:

git clone https://github.com/Comradehacker1120/Pro-phish-hack
cd Pro-phish-hack



Install Dependencies 🔄: Run to auto-install php, ssh, and Python modules:

python3 CmdPhish-HackPro.py



Set Up Tunneling 🌐:





Tool auto-downloads Cloudflared, LocalXpose.



For LocalXpose, get auth token from localxpose.io.



LocalHostRun/Serveo: SSH keys auto-configured.



Termux Users 📱: Grant storage permissions:

termux-setup-storage



Email Setup (Optional) 📧: Create files/email.json:

{"email": "your-email@gmail.com", "password": "your-app-password", "receiver": "receiver-email@gmail.com"}

Use Gmail app password.

Usage 🚀





Run Tool ▶️:

python3 CmdPhish-HackPro.py



Select Template 📋: Choose a template (e.g., 01 for first option) or use:

python3 CmdPhish-HackPro.py -o 60



Choose Tunneler 🌐: Select Cloudflared, LocalXpose, etc., or specify:

python3 CmdPhish-HackPro.py -t loclx



Configure Options ⚙️:





Port 🔢: -p 9090



Redirect URL 🔗: -u https://example.com



Custom Files 🗂️: Select custom option, provide directory



URL Masking 🎭: Follow prompts for custom URLs



Monitor Credentials 📊:





URLs generated for sharing.



Credentials saved in .site/usernames.txt, .site/ip.txt, and .creds.txt (home or /sdcard for Termux).



Email notifications if configured.



Exit 🛑: Press Ctrl+C to stop.

Command-Line Options 📝







Option



Description



Example





-p



Port (default: 8080)



-p 9090





-o



Template index



-o 60





-t



Tunneler (e.g., loclx)



-t loclx





-r



LocalXpose region



-r us





-s



LocalXpose subdomain



-s custom





-u



Redirect URL



-u https://example.com





-m



Mode (e.g., test)



-m test





-e



Troubleshoot tunneler



-e cloudflared





--nokey



LocalHostRun without SSH key



--nokey





--kshrt



Show kshrt URL



--kshrt





--noupdate



Skip update check



--noupdate

Troubleshooting 🛠️





No Internet 🌐: Check with ping google.com.



Tunneling Fails 🔌: Verify cloudflared/loclx installation, LocalXpose token, or SSH keys.



PHP Issues 💻: Ensure PHP installed (php -v), port free (netstat -tuln | grep 8080).



Termux Storage 📱: Run termux-setup-storage.



Email Issues 📧: Check email.json and Gmail app password.

Notes 📋





Ethical Use ⚖️: For authorized testing only. Misuse is prohibited.



Updates 🔄: Auto-checks unless --noupdate used. Update via:

git pull https://github.com/Comradehacker1120/Pro-phish-hack



Credits 🙌: Original by KasRoudra (2021-2024), modified by CMDHCK (2025), inspired by Zphisher, MaskPhish, AdvPhishing.

License 📜

MIT License. See LICENSE file.

Disclaimer ⚠️

Developers are not liable for misuse. Use responsibly on authorized systems only.
