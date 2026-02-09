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

