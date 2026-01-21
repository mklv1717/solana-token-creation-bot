# 🚀 Create New Repository in GitHub Desktop - Step by Step

## ⚠️ IMPORTANT: Security Check First!

Before creating the repository, make sure these **sensitive files are NOT uploaded**:
- ❌ `config.json` (contains your bot token, private keys, API keys)
- ❌ `tokens.json` (contains your token data)
- ❌ `wallets.json` (contains wallet information)

✅ These files are already in `.gitignore`, so they will be automatically excluded.

---

## 📋 Step-by-Step Guide

### ⚠️ IMPORTANT: This Directory Already Has Git

Since this folder is already connected to your old GitHub account, you have **2 options**:

**Option A: Remove old Git connection (Recommended for GitHub Desktop)**
**Option B: Change remote URL (Advanced)**

We'll use **Option A** - it's easier with GitHub Desktop.

---

### Step 1: Remove Old Git Connection

1. **Close GitHub Desktop** (if open)
2. Open **File Explorer**
3. Navigate to: `C:\Users\User\Desktop\tgbot17`
4. **Show hidden files:**
   - Click **"View"** tab
   - Check **"Hidden items"**
5. **Delete the `.git` folder:**
   - Right-click `.git` folder
   - Click **"Delete"**
   - Confirm deletion

✅ This removes the connection to your old repository but **keeps all your files**.

---

### Step 2: Open GitHub Desktop

1. Launch **GitHub Desktop**
2. **Sign out** of old account (if needed):
   - Click **"File"** → **"Options"** → **"Accounts"**
   - Click **"Sign out"**
3. **Sign in** with your **new account**

---

### Step 3: Add Existing Repository

1. Click **"File"** → **"Add Local Repository"**
   - Or click **"+"** button → **"Add Existing Repository"**

2. Click **"Choose..."** button

3. Navigate to and select: `C:\Users\User\Desktop\tgbot17`

4. Click **"Add Repository"**

---

### Step 4: Create New Repository on GitHub

1. In GitHub Desktop, you should see your repository
2. Click **"Publish repository"** button (top right)
   - Or: **"Repository"** → **"Publish Repository"**

3. **Repository settings:**
   ```
   Name: solana-token-creation-bot
   Description: Automated Telegram bot for creating Solana SPL tokens and managing listings on Pump.fun, Axiom Trade, and BullX
   Keep this code private: UNCHECKED (make it public)
   ```

4. Click **"Publish Repository"**

---

### Step 3: Verify Files to Commit

1. GitHub Desktop will show all files in the left panel
2. **Check that these files are NOT listed:**
   - ❌ `config.json`
   - ❌ `tokens.json`
   - ❌ `wallets.json`

3. **Files that SHOULD be listed:**
   - ✅ `main.py`
   - ✅ `README.md`
   - ✅ `LICENSE`
   - ✅ `requirements.txt`
   - ✅ `config.example.json`
   - ✅ `.gitignore`
   - ✅ `API_SETUP.md`
   - ✅ `SOLANA_SETUP.md`
   - ✅ `ADD_GITHUB_TOPICS.md` (optional)
   - ✅ `QUICK_TOPICS_GUIDE.md` (optional)

---

### Step 4: Make Initial Commit

1. At the bottom left, you'll see a text box for commit message
2. Type: `Initial commit: Solana Token Creation Bot`
3. Click **"Commit to main"** button

---

### Step 5: Publish to GitHub

1. After committing, you'll see a **"Publish repository"** button
2. Click it
3. **Repository settings:**
   - ✅ **Name:** `solana-token-creation-bot`
   - ✅ **Description:** `Automated Telegram bot for creating Solana SPL tokens and managing listings on Pump.fun, Axiom Trade, and BullX`
   - ✅ **Keep this code private:** **UNCHECKED** (make it public for sale)
   - ✅ **Organization:** Leave as your username

4. Click **"Publish Repository"**

---

### Step 6: Verify Upload

1. Go to: `https://github.com/YOUR_NEW_USERNAME/solana-token-creation-bot`
2. **Check that:**
   - ✅ All files are there
   - ❌ `config.json` is **NOT** visible
   - ❌ `tokens.json` is **NOT** visible
   - ❌ `wallets.json` is **NOT** visible

---

## 🔍 Double-Check Before Publishing

### ✅ Files That MUST Be Included:
- [ ] `main.py`
- [ ] `README.md`
- [ ] `LICENSE`
- [ ] `requirements.txt`
- [ ] `config.example.json`
- [ ] `.gitignore`
- [ ] `API_SETUP.md`
- [ ] `SOLANA_SETUP.md`

### ❌ Files That MUST NOT Be Included:
- [ ] `config.json` (sensitive - bot token, private keys)
- [ ] `tokens.json` (user data)
- [ ] `wallets.json` (wallet data)

---

## 🎯 After Publishing

### 1. Add Topics (Tags)
1. Go to your repository on GitHub
2. Click **⚙️** next to "About"
3. Add topics:
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
   solana-blockchain
   token-launch
   trading-bot
   ```

### 2. Update Repository Description
- Click **⚙️** next to "About"
- Add description: `Automated Telegram bot for creating Solana SPL tokens and managing listings on Pump.fun, Axiom Trade, and BullX. Fully functional with multi-platform API integration.`

### 3. Add Contact Info
- Make sure `README.md` includes: `Telegram: @usdt1717usdt`

---

## 🚨 Troubleshooting

### Problem: "config.json" appears in files to commit
**Solution:**
1. Check that `.gitignore` contains `config.json`
2. If it does, the file might already be tracked
3. In GitHub Desktop: Right-click `config.json` → **"Ignore"**

### Problem: Can't publish repository
**Solution:**
1. Make sure you're logged into GitHub Desktop with your new account
2. Check your internet connection
3. Try: **"Repository"** → **"Push"** after creating the repo

### Problem: Files missing after publish
**Solution:**
1. Make sure you committed all files before publishing
2. Check the "Changes" tab in GitHub Desktop
3. Commit any remaining files

---

## 📝 Quick Checklist

- [ ] Opened GitHub Desktop with new account
- [ ] Created new repository
- [ ] Verified `config.json` is NOT in files to commit
- [ ] Made initial commit
- [ ] Published repository
- [ ] Verified files on GitHub (sensitive files NOT visible)
- [ ] Added topics to repository
- [ ] Updated repository description

---

## 🎉 Done!

Your repository is now live on GitHub with your new account!

**For questions: Telegram: @usdt1717usdt**
