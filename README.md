
# Getting Started with This Repository

Welcome! Follow these steps to set up your local environment and contribute easily.

## 1. Clone the repository

Open your terminal and run:

```bash
git clone git@github.com:Nityam713/blogs.git
cd blogs
```

> **Note:** This uses SSH, so make sure your SSH key is set up (see below).

---

## 2. Set up SSH keys (only once per computer)

### a. Check if you already have an SSH key

Run:

```bash
ls ~/.ssh/id_ed25519.pub
```

If you see a file path, you have an SSH key. Skip to step 3.

If not, generate one:

```bash
ssh-keygen -t ed25519 -C "your_email@example.com"
```

- When prompted, press Enter to accept defaults.
- Leave the passphrase empty (just press Enter twice).

### b. Copy your public SSH key

```bash
cat ~/.ssh/id_ed25519.pub
```

Copy the output (starts with `ssh-ed25519`).

### c. Add the SSH key to GitHub

- Go to [https://github.com/settings/keys](https://github.com/settings/keys)
- Click **New SSH key**
- Paste your copied key and save

---

## 3. Verify SSH connection to GitHub

```bash
ssh -T git@github.com
```

You should see:

```
Hi <your-github-username>! You've successfully authenticated...
```

---

## 4. Working with branches

- To create a new branch and switch to it:

```bash
git checkout -b your-branch-name
```

- To switch to an existing branch:

```bash
git checkout branch-name
```

---

## 5. Pull latest changes

Before you start working, always pull the latest changes:

```bash
git pull origin main
```

---

## 6. Commit and push your changes

```bash
git add .
git commit -m "Your descriptive commit message"
git push origin your-branch-name
```

---

## 7. Create a Pull Request on GitHub

After pushing your branch, go to GitHub and create a Pull Request to merge your changes into `main`.

---

**If you face any issues or have questions, feel free to ask!*