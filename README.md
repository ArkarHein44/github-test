- Use `git status` to list all new or modified files that haven't yet been committed.
> [!NOTE]
> Red files mean modified.
> <br/>
> Green files mean staged.
> <br/>
> White filees mean committed.
- Use `git add <file>` to add modified file to staging. Use `git add * || git add .` for all files.
- Use `git rm --cached <file>` to unstage. Use `git rm --cached * || git rm --cached .` to unstage all files.
- Use `git commit -m comment` to commit. Like `git commit -m "first commit"`. `-m` m flag used to provide a commit message.
- Use `git log` to track a branch's commit history. Git will show you commit-id, Author and Date for each commit. But it's can confuse for many commits.
- Use `git log --oneline` to track commit history with one line clean (commit-hash and comment only).
- Use `git checkout commit-hash` to navigate the commit of you used specific commit of commit hash. It will delete all files, codes and commits before your checking out of commit. If you want to go back on branch use `git checkout branch_name` like `git checkout master`. Use `Ctrl+shift+C` to copy text from terminal.
- Use `git revert commit-hash` to revert commit as new commit. It'l opened with text editor like vim or nano and you can edit commit name, save and apply. git checkout and git revert are safe because it doesn't modified original commits.
- Use `git reset commit-hash --hard` to delete all commits under commit-hash you used.Pleause note that, it'l delete forever.It's dangerous.
- Use `git branch -a` to check all branches on repo. * is current branch.
- Use `git branch branch_name` to create new branch.Note that all entire codes will contain on new branch. If you want to create or delete branch, you must be on original branch (main or master). you can switch branch with `git checkout branch_name`. 
- Use `git branch -D branch_name` to delete branch.
- short hand for creating and checking out new branch with one line of code `git checkout -b branch_name`.
- To merge main or master with other branch you need to commit your codes first.You must be on main branch and use `git merge branch_name`.
- If two or more branches merge same file to main branch can cause merge conflic.A "merge conflict" in Git occurs when you try to merge changes from two different branches into one, but there are conflicting edits made to the same file in both branches, causing Git to be unable to automatically combine them, requiring manual intervention to resolve the issue by choosing which changes to keep.
- Use `git push -u origin branch_name` to push your git folder to github.
- Use `git push origin --delete branch_name` to delete branch on github
- Use `git clone repo` to clone github repo on your machine.
