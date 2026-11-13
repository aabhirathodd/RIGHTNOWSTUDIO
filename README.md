# Right Now Studio — Portfolio Website

This repository contains the complete static website files for **rightnowstudio.in** (Abhishek Rathod — Industrial Designer).

---

## 🚀 How to Publish on GitHub Pages (Free with Custom Domain)

### Step 1: Create a GitHub Repository
1. Log into your GitHub account at [github.com](https://github.com).
2. Click the **+** icon in the top right corner and select **New repository**.
3. Name your repository (for example, `portfolio` or `rightnowstudio`).
4. Set it to **Public**.
5. Do NOT initialize with a README (you already have this folder).
6. Click **Create repository**.

---

### Step 2: Upload Files to the Repository

#### Option A: Using Git (Command Line)
In this folder (`C:\Users\Hp\.gemini\antigravity\scratch\rightnowstudio`), run:
```bash
git init
git add .
git commit -m "Initial commit of Right Now Studio portfolio"
git branch -M main
git remote add origin https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPO_NAME.git
git push -u origin main
```

#### Option B: Drag and Drop (Via GitHub Website)
1. On your newly created GitHub repository page, click **uploading an existing file**.
2. Drag and drop all the files and folders from this directory into the GitHub browser window.
3. Click **Commit changes**.

---

### Step 3: Enable GitHub Pages & Custom Domain
1. In your GitHub repository, click on **Settings** (top tab).
2. On the left sidebar, click **Pages**.
3. Under **Build and deployment**:
   - **Source:** Deploy from a branch
   - **Branch:** `main` / `root`
   - Click **Save**.
4. Scroll down to **Custom domain**:
   - Because the `CNAME` file is already in your repository, `rightnowstudio.in` should be pre-populated.
   - Check the box for **Enforce HTTPS** (this generates your free SSL certificate within a few minutes).

---

### Step 4: Configure Your Domain DNS (Where you bought `rightnowstudio.in`)
Log into your domain registrar (GoDaddy, Namecheap, Google Domains / Squarespace, BigRock, Hostinger, etc.) and go to **DNS Management**:

1. **Add 4 `A` Records for the Root Domain (`@`):**
   - **Type:** `A` | **Host/Name:** `@` | **Value:** `185.199.108.153`
   - **Type:** `A` | **Host/Name:** `@` | **Value:** `185.199.109.153`
   - **Type:** `A` | **Host/Name:** `@` | **Value:** `185.199.110.153`
   - **Type:** `A` | **Host/Name:** `@` | **Value:** `185.199.111.153`

2. **Add 1 `CNAME` Record for `www`:**
   - **Type:** `CNAME` | **Host/Name:** `www` | **Value:** `YOUR_GITHUB_USERNAME.github.io.`

Once DNS propagates (usually 5–30 minutes), your custom domain `https://rightnowstudio.in` will load your portfolio securely and completely free!
