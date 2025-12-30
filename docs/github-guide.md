# GitHub Guide for PADM-GP 2163

This guide helps you get started with GitHub for assignments 2, 4, and 6.

---

## Why GitHub?

1. **Version control** - Track changes to your work over time
2. **Professional skill** - Used widely in data analysis and tech policy
3. **Collaboration** - Easy to share and get feedback
4. **Accountability** - Commit history shows your work progression

---

## One-Time Setup (15 minutes)

### Step 1: Create a GitHub Account

1. Go to [github.com](https://github.com)
2. Click "Sign Up"
3. Use your NYU email for educational benefits
4. Choose a professional username (e.g., `jsmith-nyu`, not `cooldude99`)

### Step 2: Install GitHub Desktop

**We recommend GitHub Desktop** - it's easier than command-line Git.

1. Download from [desktop.github.com](https://desktop.github.com)
2. Install and open it
3. Sign in with your GitHub account
4. When asked, use your real name and NYU email for commits

### Alternative: VS Code

If you use VS Code, it has built-in Git support. See [VS Code Git Guide](https://code.visualstudio.com/docs/sourcecontrol/overview).

---

## For Each Assignment

### Step 1: Accept the Assignment

1. Click the assignment link on Brightspace (e.g., "Assignment 2 - GitHub Link")
2. This creates YOUR private copy of the assignment repository
3. Only you and the instructor can see it

### Step 2: Clone to Your Computer

1. Open GitHub Desktop
2. Click "Clone a repository from the Internet"
3. Find your assignment repo (e.g., `assignment-2-yourname`)
4. Choose where to save it on your computer
5. Click "Clone"

### Step 3: Do Your Work

1. Open the folder on your computer
2. Read the `README.md` for instructions
3. Edit the template files or add your own
4. Save your work as you go

### Step 4: Commit Your Changes

"Committing" is like saving a snapshot of your work.

1. Open GitHub Desktop
2. You'll see your changed files listed
3. Write a short summary (e.g., "Added Part 1 analysis")
4. Click "Commit to main"

**Commit frequently** - at least once per work session. This shows your progress.

### Step 5: Push to GitHub

"Pushing" uploads your commits to GitHub.

1. Click "Push origin" in GitHub Desktop
2. Your work is now backed up online
3. The instructor can see your progress

### Step 6: Submit

**Before the deadline:**
1. Make sure all your files are committed and pushed
2. Check github.com to verify your files are there
3. Post a confirmation on Brightspace if required

---

## File Organization

Your repository should look like this:

```
assignment-2-yourname/
├── README.md              # Instructions (don't edit)
├── data/                  # Provided datasets
│   └── jolts_data.csv
├── output/                # Your graphs go here
│   ├── graph1_quits_layoffs.png
│   └── graph2_beveridge.png
├── analysis.pdf           # Your written analysis
└── code/                  # Optional: your code
    └── analysis.R
```

---

## Common Issues

### "I made changes but GitHub Desktop shows nothing"

- Make sure you saved the file
- Make sure you're looking at the right repository in GitHub Desktop

### "I can't push - authentication error"

- Go to GitHub Desktop → Preferences → Accounts
- Sign out and sign back in

### "I accidentally committed something wrong"

- Don't panic - we can see all versions
- Make the correction and commit again with a note like "Fixed error in Part 2"

### "It says there's a conflict"

- This usually happens if you edited on two computers
- Ask for help in office hours - conflicts are fixable

---

## Best Practices

1. **Commit often** - Small, frequent commits are better than one giant commit at the end
2. **Write clear messages** - "Completed Part 2 graphs" is better than "stuff"
3. **Don't commit giant files** - Keep data files under 50MB
4. **Check before deadline** - Verify your files are on github.com, not just your computer

---

## Getting Help

- **Office Hours:** Best place for GitHub questions
- **GitHub Docs:** [docs.github.com](https://docs.github.com)
- **YouTube:** Search "GitHub Desktop tutorial"

---

## FAQ

**Q: Can I use the command line instead of GitHub Desktop?**
A: Yes, if you're comfortable with it. Same workflow: clone, commit, push.

**Q: What if I'm already familiar with Git?**
A: Great! Use whatever workflow you prefer. Just make sure commits are pushed before the deadline.

**Q: Is my repository private?**
A: Yes. Only you and the instructor can see it.

**Q: Can I collaborate with classmates?**
A: You can discuss concepts, but each person must submit their own repository with their own work.

**Q: What if I miss the deadline?**
A: Late pushes are timestamped. See syllabus for late policy.

---

*Last updated: [Date]*
