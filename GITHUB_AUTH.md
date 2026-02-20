# GitHub Authentication Setup

GitHub no longer accepts passwords for Git operations. You need to use a **Personal Access Token (PAT)**.

## Step 1: Create a Personal Access Token

1. Go to GitHub: https://github.com/settings/tokens
2. Click **"Generate new token"** → **"Generate new token (classic)"**
3. Give it a name: "Portfolio Deployment"
4. Select expiration: Choose how long it should last (90 days, 1 year, etc.)
5. **Select scopes:** Check the box for **`repo`** (this gives full repository access)
6. Click **"Generate token"** at the bottom
7. **COPY THE TOKEN IMMEDIATELY** - you won't be able to see it again!

## Step 2: Use the Token When Pushing

When you run `git push`, it will ask for:
- **Username:** Your GitHub username (`jonathanavillegas`)
- **Password:** Paste your Personal Access Token (NOT your GitHub password)

## Alternative: Use SSH (More Secure, One-Time Setup)

If you prefer SSH keys (no need to enter token each time):

1. Generate SSH key:
   ```bash
   ssh-keygen -t ed25519 -C "your_email@example.com"
   ```
   (Press Enter to accept default location, optionally set a passphrase)

2. Copy your public key:
   ```bash
   cat ~/.ssh/id_ed25519.pub
   ```

3. Add to GitHub:
   - Go to https://github.com/settings/keys
   - Click "New SSH key"
   - Paste the key and save

4. Change remote URL to use SSH:
   ```bash
   git remote set-url origin git@github.com:jonathanavillegas/jonathanvillegas.github.io.git
   ```

Then `git push` will work without entering credentials.


