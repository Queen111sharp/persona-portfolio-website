# Git and GitHub workflow for this assignment

Use these steps after downloading the portfolio website files. Commands are written for Git Bash, macOS Terminal, or a Linux terminal.

## 1. Create a GitHub repository

1. Sign in at https://github.com.
2. Select **New repository**.
3. Name it `personal-portfolio-website`.
4. Choose Public if your instructor needs to view it.
5. Do not initialize it with a README or .gitignore (the project already contains both).
6. Create the repository and copy its HTTPS URL.

## 2. Put the website files together

Your local project folder should contain:

```text
index.html
style.css
script.js
profile.jpg
README.md
.gitignore
```

Copy the four website files (`index.html`, `style.css`, `script.js`, `profile.jpg`) from your portfolio ZIP into this folder. Add the supplied `README.md` and `.gitignore`.

## 3. Initialize Git and make at least five meaningful commits

Open a terminal in the project folder and run:

```bash
git init
git branch -M main
git add index.html
git commit -m "Create portfolio homepage structure"

git add style.css
git commit -m "Add responsive portfolio styling"

git add script.js
git commit -m "Add mobile navigation interactions"

git add profile.jpg
git commit -m "Add profile photo to homepage"

git add README.md .gitignore
git commit -m "Document project and add gitignore"
```

These are five separate commits. If Git asks you to identify yourself, configure your own name and email:

```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

Use the same email you use for GitHub if you want commits associated with your GitHub account.

## 4. Connect and push to GitHub

Replace the URL below with the HTTPS URL of your own repository:

```bash
git remote add origin https://github.com/YOUR-USERNAME/personal-portfolio-website.git
git push -u origin main
```

## 5. Create a feature branch and make an improvement

```bash
git switch -c feature/update-portfolio-content
```

Make a real improvement. For example, personalize the About text in `index.html`, then run:

```bash
git add index.html
git commit -m "Personalize portfolio introduction"
git push -u origin feature/update-portfolio-content
```

## 6. Open a pull request

1. Open your repository on GitHub.
2. Select **Compare & pull request** for `feature/update-portfolio-content` (or open Pull requests → New pull request).
3. Set the base branch to `main` and compare branch to `feature/update-portfolio-content`.
4. Title it `Personalize portfolio introduction`.
5. Explain what you changed, then create the pull request.
6. Review the changes. Merge the pull request into `main`.
7. If GitHub offers to delete the feature branch, you may delete it after merging.

## 7. Confirm the merge locally

```bash
git switch main
git pull origin main
git log --oneline --graph --all
```

## 8. Evidence to submit

Capture screenshots showing:

- Your GitHub repository page and file list.
- The commit history showing at least five meaningful commits.
- The feature branch.
- The pull request page showing it was merged.
- Your terminal's `git log --oneline --graph --all` output.

Submit these items:

- GitHub repository URL
- Merged pull request URL
- Screenshot of commit history
- Short explanation of the Git workflow

## Short Git workflow explanation (edit to match what you actually did)

I created a GitHub repository for my personal portfolio website and initialized Git in my local project folder. I added the website files in stages and made separate commits with descriptive messages. I pushed the `main` branch to GitHub, created a feature branch for an improvement, committed and pushed that change, and opened a pull request. After reviewing the changes, I merged the pull request into `main` and synchronized my local branch.

**Important:** Do not submit URLs or screenshots until you have actually created the repository, pushed the commits, and merged the pull request. Replace all example usernames, names, and email addresses with your own details.
