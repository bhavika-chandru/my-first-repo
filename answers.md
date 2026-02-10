## Part 3: Your First Commit

**1. What command shows you the current state of your repository?**  
git status

**2. What command stages readme.txt for commit?**  
git add readme.txt

**3. What command commits with the message "Add readme file"?**  
git commit -m "Add readme file"

**4. What command shows your commit history?**  
git log

## Part 3: Your First Commit

### 1. What command shows you the current state of your repository?
`git status`

### 2. What command stages readme.txt for commit?
`git add readme.txt`

### 3. What command commits with the message "Add readme file"?
`git commit -m "Add readme file"`

### 4. What command shows your commit history?
`git log`


---

## Part 4: Make Changes

### 1. Edit readme.txt and add a new line of text
**Command used:**  
`echo "I add a nre new line because why not" >> readme.txt`

### 2. What does git status show now?
It shows that **readme.txt is modified** and the changes are **not staged** yet.

### 3. Stage and commit your changes
`git add readme.txt`  
`git commit -m "Update readme with a new line of text"`

### 4. How many commits do you have now?
Run:  
`git log --oneline`  
Write your number after running the command.


---

## Part 5: Exploration

### 1. What does `git diff` do?
`git diff` shows the differences between your working directory and the last commit or staged version.  
It highlights what changed line-by-line before committing.

### 2. What does `git log --oneline` do?
`git log --oneline` shows a short, condensed commit history with one commit per line.


---

## Part 6: Working with Branches

### 1. What command lists all branches in your repository?
`git branch`

### 2. What command creates a new branch called feature-script?
`git branch feature-script`

### 3. What command switches to the feature-script branch?
`git switch feature-script`

### 4. What single command creates and switches to a new branch called dev?
`git switch -c dev`

### 5. Switch back to the feature-script branch
`git switch feature-script`

### 6. Verify you are on the correct branch
`git branch`  
(The current branch has a `*` next to it.)

## Part 8: Merge Branches

### 1. Switch back to the main branch
`git switch main`

### 2. List the files in your directory. Is install.sh present? Why or why not?
**Command:**
`ls`

**Answer:**  
Before merging, `install.sh` is **not present** on `main` because it was created on the `feature-script` branch, and branches keep changes separate until you merge them.

### 3. What command merges feature-script into main?
`git merge feature-script`

### 4. List the files again. What changed?
**Command:**
`ls`

**Answer:**  
After merging, `install.sh` **appears** in the `main` branch because the changes from `feature-script` were merged into `main`.

### 5. Check your commit history. What do you observe?
**Command:**
`git log --oneline --graph --decorate`

**Answer:**  
The commits from `feature-script` now show up in the history of `main`. You may also see a merge commit depending on how the merge was performed.

### 6. What command deletes the feature-script branch after merging?
`git branch -d feature-script`

## Part 9: Push to GitHub

### 1. What command links your local repo to GitHub?
`git remote add origin https://github.com/YOUR-USERNAME/my-first-repo.git`

### 2. What command pushes your commits to GitHub?
`git push -u origin main`

### 3. Refresh your GitHub page. What do you see?
I see all my project files (such as `readme.txt`, `install.sh`, and `answers.md`) uploaded to the repository, along with the commit history from my local machine.

## Part 10: Delete and Clone

### 1. Navigate out of your project folder
`cd ..`

### 2. What command deletes the local repository folder?
`rm -rf my-first-repo`

### 3. What command clones your repository from GitHub?
`git clone https://github.com/bhavika-chandru/my-first-repo.git`

### 4. Navigate into the cloned folder and verify your files are there
`cd my-first-repo`  
`ls`  

I can see all the files that were pushed to GitHub, such as `readme.txt`, `install.sh`, and `answers.md`.
