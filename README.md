# Rain of Code

Welcome to **Rain of Code**, a coding event by **Sceptix Club**.

You'll submit all your work to this repository as a Pull Request (PR). Judges review each PR to see your code, your commits, and your progress, so follow the steps below carefully.

## Before You Start

You need:

1. A **GitHub account**. Sign up at [github.com](https://github.com) if you don't have one.
2. **Git** installed on your computer. Download it from [git-scm.com](https://git-scm.com/downloads).
   Check that it's installed:
   ```bash
   git --version
   ```
3. Your name and email set in Git (use the email on your GitHub account):
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "you@example.com"
   ```

## How to Submit Your Work

### Step 1: Fork this repository

Click the **Fork** button in the top-right corner of this page:
**https://github.com/sceptix-club/RainOfCode**

This makes your own copy of the repo under your GitHub account.

### Step 2: Clone your fork

On **your fork**, click the green **Code** button and copy the URL. Then run:

```bash
git clone https://github.com/<your-username>/RainOfCode.git
cd RainOfCode
```

### Step 3: Create a branch

Name the branch after your team (lowercase, hyphens, no spaces):

```bash
git checkout -b <team-name>
```

Example: `git checkout -b code-crushers`

### Step 4: Add your work in your own folder

Put **all** your files inside `submissions/<team-name>/`:

```
RainOfCode/
└── submissions/
    └── <team-name>/
        ├── README.md      (required, see template below)
        └── ...your code
```

> **Important:** Don't edit or delete anything outside your own folder. PRs that touch other teams' files or the root files may be rejected.

### Step 5: Commit often

Commit as you go instead of making one big commit at the end. Judges look at your commit history to see how your work progressed.

```bash
git add .
git commit -m "Add login page"
```

Write commit messages that say what you changed, like `Add login page` or `Fix score calculation bug`. Avoid messages like `update` or `final`.

### Step 6: Push to your fork

```bash
git push origin <team-name>
```

### Step 7: Open a Pull Request

1. Go to your fork on GitHub. You should see a **Compare & pull request** button. Click it.
2. Check that the PR is going from your fork's `<team-name>` branch into `sceptix-club/RainOfCode` on the `main` branch.
3. Set the **title** to:
   ```
   [Submission] <Team Name>
   ```
4. Fill in the description with the [PR template](#pr-description-template) below.
5. Click **Create pull request**.

### Step 8: Keep pushing updates

You don't need a new PR for updates. Anything you push to the same branch shows up in your open PR automatically:

```bash
git add .
git commit -m "Improve UI"
git push origin <team-name>
```

**Open only one PR per team.**

## Team README Template

Put a `README.md` inside `submissions/<team-name>/` with this content:

```markdown
# <Project Name>

## Team
- Name 1 (@github-username)
- Name 2 (@github-username)

## What it does
A short description of your project.

## Tech stack
Languages, frameworks, libraries used.

## How to run
Step-by-step commands to run your project.

## Screenshots / Demo
(optional) Images or a link to a demo video.
```

## PR Description Template

Copy this into your PR description:

```markdown
**Team Name:**
**Team Members:** @user1, @user2
**Project Title:**

### Summary
What did you build?

### How to run
Short steps, or "see submissions/<team-name>/README.md"

### Demo
Link to a video, deployment, or screenshots (optional)
```

## How Judging Works

Judges will review your Pull Request, including:

- **Working code:** does it run and do what it says?
- **Commit history:** steady progress and clear commit messages
- **Documentation:** a clear team README with run instructions
- **Code quality:** readable and well organised
- **Following the rules:** files in the right folder, one PR per team

Only commits pushed before the deadline count. Anything pushed after that won't be judged.

## Rules

- One PR per team.
- Keep all your files inside `submissions/<team-name>/`.
- Don't modify other teams' folders or the root files.
- Don't commit `node_modules/`, virtual environments, `.env` files, API keys, or passwords.
- Plagiarism or copying another team's work gets you disqualified.
- Be respectful. Don't comment on or interfere with other teams' PRs.

## Common Problems

| Problem | Fix |
|---|---|
| `Permission denied` when pushing | You're pushing to the main repo instead of your fork. Run `git remote -v` and make sure `origin` points to **your** fork. |
| No "Compare & pull request" button | Open the **Pull requests** tab of the main repo, click **New pull request**, then **compare across forks**, and pick your fork and branch. |
| Accidentally committed a secret or API key | Remove it, commit again, and **revoke or regenerate the key**. Deleting it from the file doesn't remove it from Git history. |
| My fork is out of date | On your fork's GitHub page, click **Sync fork** and then **Update branch**, then run `git pull origin main`. |

Still stuck? Ask an organiser or a volunteer at the event.

Happy coding!
