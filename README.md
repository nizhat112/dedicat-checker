# dedicat-checker
 Server Credential Checker

A powerful Python tool for scanning and checking server credentials over multiple ports. Designed for system administrators, penetration testers, and IT professionals.

---

## 🔧 Features

- ✅ Check **SSH access** (port 22) using `paramiko`
- 🌐 Check **HTTP access** (ports 80 and 443) using `aiohttp` with basic authentication
- 🔍 Scan and validate **open ports** (22, 80, 443, 3389, 1080, 8080, 3128, 9000, 8081, etc.)
- ⚡ **Asynchronous** and **multithreaded** for high-speed scanning
- 📁 Select your server list via a **GUI file dialog**
- 🪟 Compatible with **Windows 8.1 and earlier**
- 📊 Real-time progress with **tqdm**
- 💾 Automatically saves valid credentials to `valid_proxies.txt`

---

## 📁 Input File Format

A simple `.txt` file containing one IP or IP:Port per line:

192.168.0.1
192.168.0.2:22
10.0.0.1:443

yaml
Копировать
Редактировать

---

## 🚀 How to Use

### 1. Install Dependencies

```bash
pip install paramiko aiohttp tqdm
2. Run the Script
bash
Копировать
Редактировать
python script_name.py
3. Select Input File
A dialog will appear — choose your .txt file with server addresses.

4. Wait for Results
The script will attempt various default username and password combinations.

Valid credentials will be saved to valid_proxies.txt.

📈 Example Output
txt
Копировать
Редактировать
192.168.0.1 admin admin123
10.0.0.1 root toor
⚠️ Disclaimer
This tool is intended for educational and authorized security testing purposes only.
Do not use it against systems you do not own or have explicit permission to test.

📬 Contact
Feel free to contribute or open an issue on GitHub if you'd like to improve this tool
