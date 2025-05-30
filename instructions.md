# Git Workflow Guide for Aesthetic CSS Framework Team
Hi guys, I have created this MD file to give you instructions about the assignment. By now I think all of you are added as collaborators, let me know if you have problems accessing the repo.

## Step-by-Step Git Workflow

### Step 1: Clone the Repository (One time only)


1. **Clone the repository**:
   ```bash
   git clone https://github.com/muoz0003/aesthetic_css_framework.git
   ```
2. **Enter the project folder**:
   ```bash
   cd aesthetic_css_framework
   ```

### Step 2: Create Your Personal Branch

Each team member creates their own branch:

**For Phil (Chuhong):**
```bash
git checkout -b chuhong-forms-tables-lists
```

**For Solomon:**
```bash
git checkout -b solomon-buttons-text-colors
```

**For Luz Helena:**
```bash
git checkout -b luz-reset-layout-utilities
```

### Step 3: Work on Your Files

1. **Open VS Code in the project folder**:
   ```bash
   code .
   ```

2. **Work on your assigned files only**:

   **Chuhong's files:**
   - `src/base/_forms.scss`
   - `src/base/_tables.scss`
   - `src/base/_lists.scss`
   - `src/utilities/_margin.scss`
   - `src/utilities/_padding.scss`

   **Solomon's files:**
   - `src/base/_buttons.scss`
   - `src/base/_text.scss`
   - `src/utilities/_colors.scss`
   - `src/utilities/_borders.scss`
   - `src/utilities/_typography.scss`

   **Luz Helena's files:**
   - `src/base/_reset.scss`
   - `src/base/_layout.scss`
   - `src/utilities/_font-sizes.scss`
   - `src/utilities/_display.scss`

### Step 4: Save and Commit Your Work

After working on your files:

1. **Check what files you've changed**:
   ```bash
   git status
   ```

2. **Add your files to staging**:
   ```bash
   git add .
   ```

3. **Commit your changes**:
   ```bash
   git commit -m "Add [Your Name]'s components - [description]"
   ```

   **Examples:**
   ```bash
   git commit -m "Add Chuhong's components - forms, tables, lists, spacing utilities"
   git commit -m "Add Solomon's components - buttons, text, colors, borders"
   git commit -m "Add Luz Helena's components - reset, layout, display utilities"
   ```

### Step 5: Push Your Branch to GitHub

```bash
git push origin your-branch-name
```

**Examples:**
```bash
git push origin chuhong-forms-tables-lists
git push origin solomon-buttons-text-colors
git push origin luz-reset-layout-utilities
```

### Step 6: Create a Pull Request (same as we did on last assignment)

1. **Go to the GitHub repository** in your web browser
2. **You'll see a yellow banner** saying "Compare & pull request" - click it
3. **If you don't see the banner**:
   - Click "Pull requests" tab
   - Click "New pull request"
   - Select your branch from the dropdown

4. **Fill out the pull request**:
   - **Title**: "Add [Your Name]'s CSS Components"
   - **Description**: List what you completed
   
   **Example for Chuhong:**
   ```
   ## Completed Components
   - ✅ Forms styling (_forms.scss)
   - ✅ Tables styling (_tables.scss) 
   - ✅ Lists styling (_lists.scss)
   - ✅ Margin utilities (_margin.scss)
   - ✅ Padding utilities (_padding.scss)
   
   ## Testing
   - Tested with different form elements
   - Verified table styling works
   - Checked spacing utilities
   ```

   **Example for Solomon:**
   ```
   ## Completed Components
   - ✅ Button styling (_buttons.scss)
   - ✅ Text elements styling (_text.scss)
   - ✅ Color utilities (_colors.scss)
   - ✅ Border utilities (_borders.scss)
   - ✅ Typography utilities (_typography.scss)
   
   ## Testing
   - Tested button variants and states
   - Verified color contrast accessibility
   - Checked utility class overrides
   ```

   **Example for Luz Helena:**
   ```
   ## Completed Components
   - ✅ CSS Reset/Normalize (_reset.scss)
   - ✅ Layout styles (_layout.scss)
   - ✅ Font size utilities (_font-sizes.scss)
   - ✅ Display utilities (_display.scss)
   
   ## Testing
   - Tested cross-browser compatibility
   - Verified responsive grid system
   - Checked flex utilities
   ```

5. **Click "Create pull request"**

---

## Important Rules

### ❌ DON'T DO THIS:
- Don't work on files that aren't assigned to you
- Don't commit to the `main` branch directly
- Don't merge your own pull requests
- Don't delete other people's code
- Don't modify `main.scss`, `_config.scss`, or `_colors.scss` (David's files)

### ✅ DO THIS:
- Only work on your assigned files
- Test your code before committing
- Write clear commit messages
- Ask for help if you're stuck
- Follow the TODO instructions in each file
- Use the variables I have created on the `/variables` folder 

---

## File Assignment Reference

| Team Member | Base Styles | Utility Classes |
|-------------|-------------|-----------------|
| **Chuhong** | `_forms.scss`, `_tables.scss`, `_lists.scss` | `_margin.scss`, `_padding.scss` |
| **Solomon** | `_buttons.scss`, `_text.scss` | `_colors.scss`, `_borders.scss`, `_typography.scss` |
| **Luz Helena** | `_reset.scss`, `_layout.scss` | `_font-sizes.scss`, `_display.scss` |
| **David** | `_typography.scss` | Variables, main.scss, demo.html |

---

## Emergency Commands

### If you made a mistake:
```bash
git reset --hard HEAD~1  # Undoes last commit
git checkout main         # Go back to main branch
git pull origin main      # Get latest changes
```

### If you're lost:
```bash
git status               # See what's happening
git branch              # See which branch you're on
git log --oneline       # See your commits
```

### If you need to start over:
```bash
git checkout main
git pull origin main
git branch -D your-branch-name  # Delete your branch
git checkout -b your-branch-name  # Create new branch
```

---

## Quick Reference Card

| Action | Command |
|--------|---------|
| Create branch | `git checkout -b branch-name` |
| See status | `git status` |
| Add files | `git add .` |
| Commit | `git commit -m "message"` |
| Push | `git push origin branch-name` |
| Switch branch | `git checkout branch-name` |
| Get latest main | `git pull origin main` |

---

## Testing Your Code

Before creating a pull request, make sure to:

1. **Open the demo.html file** in your browser
2. **Check that your components look good**
3. **Test different screen sizes** (mobile, tablet, desktop)
4. **Verify no errors** in browser console (F12)

---

## David's Final Integration Steps

After everyone's pull requests are approved:

1. **I will merge all branches into main**
2. **Test the complete framework**
3. **Compile the final CSS** using Sass
4. **Update demo.html** if needed
5. **Create final release**
6. **Submit the assignment**

---

## Troubleshooting

### "Permission denied" error:
- Make sure you're a collaborator on the repository
- Check that you're logged into the correct GitHub account

### "Branch already exists" error:
```bash
git checkout existing-branch-name
```

### "Nothing to commit" message:
- Make sure you saved your files in VS Code
- Check that you're working on the right files

### Pull request conflicts:
- Ask David for help - don't try to resolve alone

---

## Need Help?

1. **Team Communication**: Use WhatsApp group

---

## VS Code Git Integration (Alternative to Command Line)

If you prefer using VS Code instead of command line:

1. **Open Source Control panel** (Ctrl+Shift+G)
2. **Stage changes** by clicking the + next to files
3. **Write commit message** in the text box
4. **Click checkmark** to commit
5. **Click "..." menu** → Push to push to GitHub

---

## Success Checklist

Before submitting your pull request, ensure:

- [ ] All your assigned files are complete
- [ ] Code follows the examples and TODO instructions
- [ ] No syntax errors in your SCSS files
- [ ] Variables are used correctly (after David pushes them)
- [ ] Commit messages are clear and descriptive
- [ ] Pull request description lists completed work
- [ ] You haven't modified files assigned to others

---

**Remember**: It's better to ask for help than to break something! The goal is to learn and create something awesome together. 

## Repository Structure Overview

```
aesthetic_css_framework/
├── src/
│   ├── base/           # Base HTML element styling
│   ├── utilities/      # Utility classes
│   ├── variables/      # Sass variables (David only)
│   └── main.scss       # Main entry point (David only)
├── dist/               # Compiled CSS output
├── examples/           # Demo files
└── README.md           # Documentation
```

Let me know if you have any questions! Best, David. 