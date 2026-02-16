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

## Steps to Creating and Merging 
1. Make changes on the branch
    - Edit your files
    - Save your work 
2. See what changed
    - Run: `git status` or `git diff` to see edits
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


## Bulma
[Bulma Documentation](https://bulma.io/documentation/)