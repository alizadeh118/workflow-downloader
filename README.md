# 📥 Download via GitHub Actions Releases

This repository allows you to download files using **GitHub Actions** and store them as **GitHub Releases**.

It is useful in restricted environments where only `github.com` is accessible.

---

## 🚀 How it works

When you push changes to this repository:

1. GitHub Actions reads a URL from `url.txt`
2. Downloads the file on GitHub’s servers
3. Creates a GitHub Release
4. Attaches the downloaded file to the release

---

## 🛠️ Setup & Usage

### 1. Fork this repository

Click the **Fork** button on GitHub to create your own copy.

---

### 2. Add your download link

Edit the file:

```
url.txt
```

Put your direct download link inside:

```
https://example.com/file.zip
```

---

### 3. Commit and push

After updating `url.txt`:

```bash
git add url.txt
git commit -m "update download link"
git push
```

---

### 4. Trigger the workflow (auto)

Every push that modifies `url.txt` will automatically:

- Read the URL from `url.txt`
- Download the file
- Create a GitHub Release
- Attach the file to the release

---

### 5. Download your file

Go to the [latest release](../../releases/latest) and download the attached file.
