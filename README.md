# 📌 CmdPhish-HackPro - Advanced Phishing Tool

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![License](https://img.shields.io/badge/License-MIT-green)
![Platform](https://img.shields.io/badge/Platform-Linux%20|%20Termux-yellow)

**CmdPhish-HackPro** is a powerful phishing tool with 70+ website templates, tunneling options, and credential capturing capabilities. Based on original work by KasRoudra, enhanced by CMDHCK.

## 🌟 Features

- 70+ phishing templates (Facebook, Instagram, GitHub, etc.)
- Multiple tunneling options (Cloudflared, LocalXpose, Serveo)
- URL masking and shortening capabilities
- Automatic IP and credential logging
- Email notification system
- Cross-platform support (Linux, Termux)
- User-friendly interface

## ⚙️ Installation

### 💻 Linux Requirements
```bash
sudo apt update
sudo apt install -y git python3 php openssh
```

### 📱 Termux Requirements
```bash
pkg update
pkg install -y git python php openssh
termux-setup-storage
```

### 📥 Install CmdPhish-HackPro
```bash
git clone https://github.com/Comradehacker1120/Pro-phish-hack
cd Pro-phish-hack
chmod +x CmdPhish-HackPro.py
python3 CmdPhish-HackPro.py
```

## 🚀 Usage Guide

1. **Run the tool**:
   ```bash
   python3 CmdPhish-HackPro.py
   ```

2. **Select a phishing template** from the menu

3. **Choose tunneling method** when prompted:
   - Cloudflared (Recommended)
   - LocalXpose
   - Serveo
   - LocalHostRun

4. **Share the generated phishing link** with your target

5. **Captured credentials** will be saved automatically in:
   - `creds.txt` - Login credentials
   - `ip.txt` - Victim IP addresses

### ⚡ Advanced Options
```bash
# Custom port (default: 8080)
python3 CmdPhish-HackPro.py -p 8081

# Specify template by number
python3 CmdPhish-HackPro.py -o 15

# Force specific tunneler
python3 CmdPhish-HackPro.py -t cloudflared

# Set redirection URL
python3 CmdPhish-HackPro.py -u https://google.com
```

## 📧 Email Configuration

To enable email notifications:
1. Edit `files/email.json`
2. Add your Gmail credentials (use app password)
```json
{
  "email": "your@gmail.com",
  "password": "your-app-password",
  "receiver": "receiver@email.com"
}
```

## 🛠 Troubleshooting

- If Cloudflared/LocalXpose fails, try reinstalling:
  ```bash
  rm -rf ~/.tunneler
  python3 CmdPhish-HackPro.py
  ```
  
- For Termux storage issues:
  ```bash
  termux-setup-storage
  ```

## ⚠️ Disclaimer

This tool is for **educational purposes only**. The developer is not responsible for any misuse. Use at your own risk and only on systems you have permission to test.

## 🙏 Credits

- Original Author: [KasRoudra](https://github.com/KasRoudra)
- Modified by: [CMDHCK](https://github.com/Comradehacker1120)
- Inspired by: Zphisher, MaskPhish, AdvPhishing

---

💡 **Pro Tip**: Always use responsibly and ethically! Consider using this tool only for penetration testing with proper authorization.

🔗 **Repository**: [https://github.com/Comradehacker1120/Pro-phish-hack](https://github.com/Comradehacker1120/Pro-phish-hack)
