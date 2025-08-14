# 🚀 EthStorage V1 Trusted Setup Ceremony Guide

This guide will help you participate in the **EthStorage V1 Trusted Setup Ceremony** 

---

## 📌 Requirements
- Ubuntu 22.04 VPS (2 vCPU, 4GB RAM, 30GB+ SSD recommended)
- Basic SSH access
- GitHub account (for authentication)

---

## 🛠 Step-by-Step Setup

### 1️⃣ Update & Install Dependencies
```
apt update && apt upgrade -y
apt install -y curl git build-essential

```

### 2️⃣ Install Node.js v18 & npm v9.2
```

curl -fsSL https://deb.nodesource.com/setup_18.x | bash -
apt install -y nodejs
npm install -g npm@9.2
```

### 3️⃣ Check Versions



node -v
npm -v

### 4️⃣ Create Temporary Directory

```
mkdir ~/trusted-setup-tmp && cd ~/trusted-setup-tmp

```
### 5️⃣ Install Phase2 CLI

```
npm install -g @p0tion/phase2cli
```

### 6️⃣ Verify CLI Installation


```
phase2cli --version
```

### 7️⃣ Authenticate with GitHub

```
phase2cli auth
```

* Follow the browser link shown in the terminal
* Login to GitHub & authorize **p0tion** to access Gists
* Return to terminal

### 8️⃣ Contribute to the Ceremony

```
phase2cli contribute -c ethstorage-v1-trusted-setup-ceremony
```

---

## 🧹 Cleanup After Contribution

```
phase2cli clean
phase2cli logout
cd ~ && rm -rf ~/trusted-setup-tmp
```

---

## 💡 Pro Tips

1. **Run commands inside a `screen` session so contribution continues if you disconnect:**


apt install -y screen
screen -S ceremony
# Run all commands inside here
# Detach with: CTRL + A then D
# Reattach with: screen -r ceremony

 **Destroy VPS after participation for maximum security**

---

✅ **You have successfully contributed to the EthStorage V1 Trusted Setup Ceremony!**

---

Ye format GitHub pe perfect lagega — commands copy-paste friendly hain, headings clear hain, aur screen ka tip bhi added hai taaki disconnect hone ka issue na ho.  

Agar tum chaGitHub-flavored clickable "Copy" button "Copy" button** वाला HTML + Markdown mix version bhi bana sakta hoon jo aur premium lage.
`
