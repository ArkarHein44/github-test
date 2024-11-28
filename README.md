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
- Use `git checkout commit-hash` to navigate the commit of you used specific commit of commit hash. It will delete all files, codes and commits before your checking out of commit. If you want to go back for last commit use `git checkout branch_name` like `git checkout master`. Use Ctrl+Shift+C to copy from treminal.
