# GitHub Profile README Upload Guide

This folder contains a GitHub profile README for Eugene Gu.

## 1. Confirm your GitHub username

The README currently assumes your GitHub username is:

```text
eugenegujing
```

If your real GitHub username is different, replace every `eugenegujing` in:

- `README.md`
- `.github/workflows/snake.yml`

Your GitHub profile repository must have the exact same name as your username.

## 2. Create the special GitHub profile repository

1. Go to <https://github.com/new>.
2. Set **Repository name** to your exact GitHub username, for example `eugenegujing`.
3. Set the repository to **Public**.
4. You may leave **Add a README file** unchecked because this folder already has one.
5. Click **Create repository**.

GitHub should show a message saying this is a special repository for your profile.

## 3. Upload from this local folder with Git

Open PowerShell in this folder:

```powershell
cd "C:\Users\Eugen\Desktop\Coding Projects\GitHub Overview User Profile"
git init
git branch -M main
git add README.md UPLOAD_GUIDE.md .github/workflows/snake.yml
git commit -m "Create GitHub profile README"
git remote add origin https://github.com/eugenegujing/eugenegujing.git
git push -u origin main
```

If your username is different, replace both parts of the remote URL:

```powershell
git remote add origin https://github.com/YOUR_USERNAME/YOUR_USERNAME.git
```

## 4. Enable the dynamic contribution graph

After pushing:

1. Open the repository on GitHub.
2. Go to **Actions**.
3. If GitHub asks you to enable workflows, click **I understand my workflows, go ahead and enable them**.
4. Open **Generate contribution graph**.
5. Click **Run workflow**.
6. Wait for it to finish, then refresh your GitHub profile.

The animation image may appear only after the first workflow run creates the `output` branch.

## 5. Quick edit checklist

Before publishing publicly, review:

- Whether you want to keep your email visible.
- Whether you want to add LinkedIn, portfolio, or project repository links.
- Whether the username `eugenegujing` is correct.
- Whether you want to remove dynamic stats if you prefer a fully static profile.
