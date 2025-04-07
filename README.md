
# CLI Node Run Full Guide (PC VPS and phone for Both)

Go to: [https://app.hyperbolic.xyz](https://app.hyperbolic.xyz)

- Click Create Account by Using ur Gmail  
- On next popup or in Settings, confirm ur phone number to get 1$ of free credits (Compulsory)  
- Go to Settings tab on Hyperbolic dashboard > Scroll down and copy ur API Key  

🔹 **Dependencies for WINDOWS & LINUX & VPS**

```bash
sudo apt update && sudo apt upgrade -y
```

🔹 **Install Python & Pip**

```bash
sudo apt install git python3 python3-pip python3-venv -y
```

🔹 **Download Node Files**

```bash
git clone https://github.com/0xmoei/chatbot-app.git
cd chatbot-app
```

🔹 **For VPS Only: Install & Start Screen**

```bash
apt install screen -y
screen -S hyperbolic
```

🔹 **Install Python Requirements**

```bash
python3 -m venv venv
source venv/bin/activate
pip install requests
```

🔹 **Configure Environment Variables**

```bash
nano chatbot.py
```

➡️ Edit this line:
```python
"Authorization": "Bearer YOUR_API_KEY_HERE"
```

Replace `YOUR_API_KEY_HERE` with your actual API key.

Save with: `CTRL + X`, then `Y`, then `Enter`

🔹 **Start Node**

```bash
python3 chatbot.py
```
✅ It will stop after 100 questions. Just run the command again to continue.

🔹 **For VPS Only: Keep Node Running in Background**

Detach:

```bash
CTRL + A + D
```

Re-attach later:

```bash
screen -r hyperbolic
```

---

## 🔶 For Next Day Run This Command

**#1 Open WSL and Put this Command**

```bash
cd chatbot-app
```

```bash
python3 chatbot.py
```

---

🧹 **Delete Node Folder (if needed)**

```bash
rm -rf ~/chatbot-app
```

---

✅ Done! You’re all set to earn running your Hyperbolic Node 🚀
```

---

Let me know if you'd like this uploaded directly to a GitHub repo or packaged in a `.md` file!
