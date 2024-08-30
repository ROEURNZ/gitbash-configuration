Here's the updated `README.BASH.md` with an image reference included:

---

# How to Set Up Version Control with GitHub on Windows

## 1. Download and Install Git Desktop and Git Bash

- [Git Desktop](https://desktop.github.com/)
- [Git Bash](https://gitforwindows.org/)

## 2. Create a New GitHub Account with Your Gmail Account

- **Username:** Choose a unique username.
- **Password:** Create a secure password.

### Enable Two-Factor Authentication (2FA)

- Use an authenticator app, SMS, or security key.

### Install Git on Windows

### Set Up System Environment Variables

- **Environment Variable:**
  ```
  C:\Program Files\Git\bin\
  ```
- **System Variable:**
  ```
  C:\Program Files\Git\cmd\
  ```

### Verify Your Git Configuration

1. Check Git version:
   ```bash
   git --version
   ```

2. Set Git username and email:
   ```bash
   git config --global user.name "Username"
   git config --global user.email "your_new_email@example.com"
   ```

3. Verify your Git configuration:
   ```bash
   git config --global user.email
   git config --global user.name
   ```

4. Generate an SSH key:
   ```bash
   ssh-keygen -t ed25519 -C "your_new_email@example.com"
   ```
   **Press Enter three times to accept the default settings.**

5. Copy SSH key to clipboard:
   ```bash
   clip < ~/.ssh/id_ed25519.pub
   ```

6. Set correct permissions on your SSH keys:
   ```bash
   ls -la ~/.ssh
   chmod 600 ~/.ssh/id_ed25519
   chmod 644 ~/.ssh/id_ed25519.pub
   ```

### Example of Commands in Git Bash

![Git Bash Commands](command.png)

---
