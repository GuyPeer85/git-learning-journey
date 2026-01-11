# My Amazing Git Learning Path - Version 2
## Commands Learned So Far
- git clone
- git status
- git add
- git commit

## Key Concepts
- Working Directory: Where you edit files
- Staging Area: Files prepared for commit
- Repository: Committed history in .git folder
## Git Reset Practice
- git reset --soft (keeps staging)
- git restore (discards working directory changes)
- git reset HEAD <file> (unstage single file - old syntax)
## Git Stash Practice
- git stash (save work temporarily)
- git stash pop (apply and delete from list)
- git stash apply (apply but keep in list)
- git stash push -m "message" (stash with description)
- git stash list (view all stashes)
- git stash clear (delete all stashes)
Modified existing file
- git stash -u (include untracked files)
Modified tracked file
- git stash -a (include all files, even ignored)
- git stash -p (interactive/selective stashing)
- git stash clear (delete all stashes - PERMANENT!)
- git stash branch <name> (create branch from stash)
## Git Log Time Filters
- git log --since="date" (commits after date)
- git log --until="date" (commits before date)
- git log --after="date" (alias for --since)
- git log --before="date" (alias for --until)
  - Relative: '1 week ago', 'yesterday', '3 days ago'
  - Absolute: '2026-01-03' or '2026-01-03 00:00'
  - Warning: Date without time uses current time!
## Git Log Author/Committer Filters
- git log --author="name" (filter by author)
- git log --committer="name" (filter by committer)
  - Uses pattern matching (partial strings work)
  - Author = who wrote the code
  - Committer = who created the commit
  - Usually same person, differs for GitHub web commits
  - Can combine with time filters
