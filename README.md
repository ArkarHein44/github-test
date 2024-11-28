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
- Use `git branch -a` to check branches on repo.
- Use `git branch branch_name` to create new branch.Note that all entire codes will contain on new branch. If you want to create new branch you must be on original branch (main or master).