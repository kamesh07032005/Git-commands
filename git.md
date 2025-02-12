

### **1. Install GitHub CLI (if not installed)**
🔹 Check if you have GitHub CLI installed:
```sh
gh --version
```
🔹 If not installed, download and install it:
- **Linux/macOS:**  
  ```sh
  sudo apt install gh  # Debian/Ubuntu
  brew install gh      # macOS (Homebrew)
  ```
- **Windows:** Download and install from [GitHub CLI](https://cli.github.com/).

---

### **2. Authenticate GitHub CLI**
Log in to GitHub from your terminal:
```sh
gh auth login
```
- Choose **GitHub.com**.
- Select **HTTPS or SSH** for authentication.
- Follow the prompts to authenticate.

---

### **3. Create a New Repository**
Run the following command:
```sh
gh repo create my-repo --public --source=. --remote=origin
```
Replace `my-repo` with your desired repository name.

#### 🔹 Options:
- `--public` → Makes the repository public (use `--private` for private repos).
- `--source=.` → Uses the current directory as the repo.
- `--remote=origin` → Automatically adds the remote URL.

---

### **4. Push Your Code to GitHub**
If your local project isn't already a Git repository, initialize it:
```sh
git init
git add .
git commit -m "Initial commit"
```

Then push it to the newly created repository:
```sh
git branch -M main
git push -u origin main
```

---

### 🎉 Done!  
Now your repository is on GitHub. You can check it by running:
```sh
gh repo view --web
