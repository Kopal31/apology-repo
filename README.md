# Apology Pull Request (Mock GitHub UI)

A customized, interactive mock GitHub Pull Request page designed to resolve communication freezes and restore peace.

## 🚀 How to Publish Privately using GitHub Pages

To keep the source code hidden from the general public while keeping the website viewable at a public URL (e.g., `https://yourusername.github.io/apology-repo`), follow these steps:

### 1. Create a Private Repository on GitHub
1. Go to [GitHub](https://github.com) and click the **+** icon in the top-right corner, then select **New repository**.
2. Set the repository name to `apology-repo`.
3. Select **Private** (so the source code remains hidden).
4. Do **not** initialize with a README, `.gitignore`, or license.
5. Click **Create repository**.

### 2. Push this Local Code to your New Repository
Open your terminal and run the following commands (replace `yourusername` with your actual GitHub username):

```bash
# Navigate to this project directory
cd /Users/kopalsoni/.gemini/antigravity/scratch/apology-repo

# Link the local repository to your remote private GitHub repository
git remote add origin git@github.com:yourusername/apology-repo.git

# Rename branch to main (if not already main)
git branch -M main

# Push the changes
git push -u origin main
```
*(Note: If you use HTTPS instead of SSH, the remote URL will be `https://github.com/yourusername/apology-repo.git`)*

### 3. Enable GitHub Pages for the Private Repository
GitHub now lets free accounts publish Pages from private repositories. 
1. In your GitHub repository page, click the **Settings** tab (the gear icon on the top right).
2. On the left sidebar, click **Pages** under the "Code and automation" section.
3. Under **Build and deployment**:
   - Source: **Deploy from a branch**
   - Branch: Select **`main`** and folder **`/ (root)`**
4. Click **Save**.

### 4. Share the Link
Within a minute or two, GitHub will build the site. You'll see a message at the top of the Pages settings tab:
> 🚀 **Your site is live at** `https://yourusername.github.io/apology-repo/`

The source code will remain completely hidden from everyone except you, but Shiva will be able to visit the URL, interact with the PR, approve, and click "Squash and merge" to see the reconciliation sequence! 🥺

---

## 🎨 What was polished in this version:
- **Pulsing Status Badge:** The "Open" indicator now has a soft, pulsing white dot to capture attention.
- **Micro-interactions:** Hovering over the Approve, Reject, and Comment buttons now triggers subtle glows and transitions matching GitHub's accent colors.
- **Smooth Navigation:** Switching between the "Conversation", "Commits", and "Files changed" tabs is now enhanced with a smooth slide-and-fade transition.
- **Animated Reviews:** Submitting a review (Approve, Request changes, Comment) now has a smooth slide-down entry animation for the comment card.
