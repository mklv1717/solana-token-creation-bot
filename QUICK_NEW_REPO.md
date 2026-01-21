# ⚡ Quick Guide: New Repository with New GitHub Account

## 🎯 Fast Method (3 Steps)

### Step 1: Remove Old Git Connection

**Option A: Using PowerShell (Fastest)**
1. Open **PowerShell** in this folder
2. Run:
   ```powershell
   Remove-Item -Recurse -Force .git
   ```

**Option B: Manual**
1. Open File Explorer
2. Go to: `C:\Users\User\Desktop\tgbot17`
3. Enable "Show hidden files" (View → Hidden items)
4. Delete the `.git` folder

---

### Step 2: Open GitHub Desktop

1. Launch **GitHub Desktop**
2. Sign in with your **new account**
3. Click **"File"** → **"Add Local Repository"**
4. Select: `C:\Users\User\Desktop\tgbot17`
5. Click **"Add Repository"**

---

### Step 3: Publish to GitHub

1. Click **"Publish repository"** button
2. Settings:
   - Name: `solana-token-creation-bot`
   - Description: `Automated Telegram bot for creating Solana SPL tokens`
   - **Keep private:** UNCHECKED ✅
3. Click **"Publish Repository"**

---

## ✅ Verify Security

After publishing, check on GitHub:
- ✅ `config.json` is **NOT** visible
- ✅ `tokens.json` is **NOT** visible  
- ✅ `wallets.json` is **NOT** visible

These files are in `.gitignore` and should be automatically excluded.

---

## 🏷️ Add Topics (After Publishing)

1. Go to your repository on GitHub
2. Click **⚙️** next to "About"
3. Add:
   ```
   solana
   telegram-bot
   cryptocurrency
   token-creation
   python
   aiogram
   blockchain
   automation
   pump-fun
   spl-token
   defi
   crypto-bot
   ```

---

**Done!** 🎉

**For questions: Telegram: @usdt1717usdt**
