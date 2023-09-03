## Staging and Commit
    a = add                           # Stage changes
    aa = add -A                       # Stage all changes, including untracked files
    ap = add -p                       # Interactively stage changes

    c = commit --verbose              # Commit with verbose output
    ca = commit -a --verbose          # Commit all changes with verbose output
    cm = commit -m                    # Commit with a specified message
    cam = commit -a -m                # Commit all changes with a specified message
    m = commit --amend --verbose      # Amend the last commit with verbose output

## Difference
    d = diff                          # Show the difference between the working directory and last commit
    ds = diff --stat                  # Show a summary of changes as a stat
    dc = diff --cached                # Show the difference between the index (staged changes) and last commit

## Status
    s = status -s                    # Show short status of changed files
    st = status                       # Show a detailed status

## Checkout and Branch
    co = checkout                     # Checkout a branch or commit
    cob = checkout -b                 # Create and checkout a new branch

## Unstage
    unstage = restore --staged        # Unstage changes from the index

## Branch Listing
    b = "!git for-each-ref --sort='-authordate' --format='%(authordate)%09%(objectname:short)%09%(refname)' refs/heads | sed -e 's-refs/heads/--'"  # List branches sorted by author date

## List Aliases
    la = "!git config -l | grep alias | cut -c 7-"  # List Git aliases

## Configuration
    config-name = config --global user.name "Your Name"                # Set global Git user name
    config-email = config --global user.email "your.email@example.com"  # Set global Git user email
    config-editor = config --global core.editor "editor"                # Set global Git text editor

## Repository Initialization
    init = init                        # Initialize a new Git repository
    clone = clone                      # Clone a remote repository

## Change Management
    git-status = status                # Alias for 'status'
    git-add = add                      # Alias for 'add'
    git-commit = commit                # Alias for 'commit'
    git-diff = diff                    # Alias for 'diff'

## Branches
    git-branch = branch                # Alias for 'branch'
    git-checkout = checkout            # Alias for 'checkout'
    git-merge = merge                  # Alias for 'merge'

## Update and Synchronize
    git-fetch = fetch                  # Alias for 'fetch'
    git-pull = pull                    # Alias for 'pull'
    git-push = push                    # Alias for 'push'

## Ignore Files
    git-ignore = "!echo 'file_or_directory_to_ignore' >> .gitignore"  # Ignore a file or directory in .gitignore

## Undo Changes
    git-reset = reset                  # Alias for 'reset'
    git-revert = revert                # Alias for 'revert'

## Others
    git-remote-add = remote add        # Alias for 'remote add'
    git-remote-list = remote -v        # Alias for 'remote -v'
    git-show = show                    # Alias for 'show'
    git-stash = stash                  # Alias for 'stash'
    git-stash-apply = stash apply      # Alias for 'stash apply'
    git-help = help                    # Alias for 'help'
