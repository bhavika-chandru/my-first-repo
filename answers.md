## Part 5: Exploration

### 1. What does `git diff` do?
`git diff` shows the **differences between your working directory and the last commit or staged version**.  
It highlights what has changed line-by-line but has **not been committed** yet.

### 2. What does `git log --oneline` do?
`git log --oneline` shows a **short, condensed history of your commits**, where each commit appears on a single line.  
It makes it easy to see commit IDs and messages at a glance.

## Part 4: Make Changes

**1. Edit readme.txt and add a new line of text**

Command used:
echo "I add a nre new line because why not" >> readme.txt

**2. What does git status show now?**

It shows that readme.txt is modified and the changes are not staged yet.

**3. Stage and commit your changes**

git add readme.txt
git commit -m "Update readme with a new line of text"

**4. How many commits do you have now?**

git log --oneline


## Part 3: Your First Commit

**1. What command shows you the current state of your repository?**  
git status

**2. What command stages readme.txt for commit?**  
git add readme.txt

**3. What command commits with the message "Add readme file"?**  
git commit -m "Add readme file"

**4. What command shows your commit history?**  
git log
