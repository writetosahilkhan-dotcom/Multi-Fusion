# Setup Instructions for GitHub and CodeRabbit

## 1. Create GitHub Repository

```bash
# Create a new repository on GitHub (via web interface or CLI)
# Then connect your local repository:

git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
git branch -M main
git push -u origin main
```

Or using GitHub CLI:
```bash
gh repo create multi-satellite-dashboard --public --source=. --remote=origin
git push -u origin main
```

## 2. Install CodeRabbit GitHub App

1. Visit: https://github.com/apps/coderabbit-ai
2. Click "Install" or "Configure"
3. Select your account/organization
4. Choose repository access:
   - Select "Only select repositories"
   - Choose your multi-satellite-dashboard repository
5. Click "Install" or "Save"

## 3. Verify CodeRabbit Setup

After installation:
- CodeRabbit will automatically review new pull requests
- Configuration is already set in `.coderabbit.yaml`
- Create a test PR to verify it's working

## 4. CodeRabbit Features Enabled

✓ Automatic code reviews on PRs
✓ High-level summaries
✓ Review poems (fun feature!)
✓ Language-specific checks (JS/TS, Python, CSS)
✓ Security and performance analysis
✓ Auto-reply in chat

## 5. Quick Commands

```bash
# Create a new branch and make changes
git checkout -b feature/your-feature
# ... make changes ...
git add .
git commit -m "Add: your feature"
git push origin feature/your-feature

# Then create a PR on GitHub - CodeRabbit will automatically review it!
```

## Notes
- CodeRabbit is free for open-source projects
- Reviews typically appear within 1-2 minutes of PR creation
- You can interact with CodeRabbit using comments like "@coderabbitai review this"
