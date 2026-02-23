# HTML & Git Notes with Doc

_Date: February 16, 2026_

## HTML Concepts
- Semantic containers: `header`, `nav`, `main`, `footer`, `section`, `article`
- Generic container: `div` (no meaning by itself, used for layout/styling)
- `header` usually holds logo, main heading, nav, intro text
- `main` holds the main unique content of the page (only one per page)

## Git Basics
Git switch is a newer command designed for switching.
- Create and switch to new branch: `git switch -c practice-branch`
- Old way to create and switch: `git checkout -b new-branch`
- Switch to an existing branch: `git switch main` (or `master`)
- Switch to a previous branch: `git switch -`
- Check current branch: `git branch` or `git status`
- Merge a branch into main:
  - `git switch main`
  - `git merge practice-branch`
- View all commits: `git log` will show new commits first
- One line per commit: `git log --oneline`

## Steps to Creating and Merging 
1. Make changes on the branch
    - Edit your files
    - Save your work 
2. See what changed
    - Run: `git status` or `git diff` to see edits before staging. This will show changes between your working directory and the last commit
    - Run: `git diff --staged` to show what's in the staging area before commit
    - Run: `git diff main BRANCH` to compare after commits
3. Stage and commit your changes
    - Stage: `git add .` (or specific files)
    - Commit: `git commit -m "TEXT"`
4. Push the branch to Github 
    - Command: `git push -u origin practice-branch`
5. OR Go back to the main branch
    - Command: `git switch main`
6. Merge the branch into main
    - `git merge practice-branch`
7. If there are no conflicts, push the updated main into Github
    - `git push`

## Delete
After everything is done, you can safely delete the local branch
- `git branch -d practice-branch`

## Reverting Commits
1. Safe way to undo a commit: `git revert`

1. Safe way (recommended for shared repos): git revert
This creates a new commit that undoes an earlier one.

Find the commit hash:
git log --oneline
Revert that commit:
git revert <commit-hash>
If it opens an editor for the message, save & close, then:
git push
Use this when the commits are already on GitHub or others may have pulled them.

2. Rewrite history (only if you’re sure): git reset
This moves your branch pointer backwards.

3. In case any files were tracked by Git and need to be removed from tracking: 

`git rm -r --cached node_modules/`

`git rm --cached .env`

See commits:
git log --oneline
Hard reset to an older commit (throws away later commits from this branch):
git reset --hard <commit-hash>
Then push with force (only if you know what you’re doing):
git push --force
Use reset --hard only on branches that are just yours and you understand that newer commits will be removed from that branch’s history.

## Bulma
[Bulma Documentation](https://bulma.io/documentation/)