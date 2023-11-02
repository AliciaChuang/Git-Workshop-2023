# Git-Workshop-2023
Slides for reference - https://docs.google.com/presentation/d/e/2PACX-1vT7nJYRovLzU8J--OhyiNsIbh__haA0gCPZLw4Nptsd4z7pfos7-8dsZdaTV8PUaukqsd4yfrMjxJkO/pub?start=false&loop=false&delayms=60000
- Have one person fork this repository on GitHub and invite others as collaborators
  - To add collaborators: Settings → Collaborators
- Have each person pull the project into their local repository
  - git clone [HTTPS url]
- Modify your functions and merge the changes
  - a merge conflict should occur. Try fixing it together with git rebase

## Challenge activities
- Create a new local branch with all the changes from main, and checkout that branch
- Make changes without committing and stash them. Then checkout main branch again
- Make additional changes to main branch and commit multiple times without pushing
- Squash all unmerged commits and push to the remote repository
- Switch back to your local branch, pop the changes and push the branch to a remote branch of the same name

## Possible Issues
- Unable to link your Git and GitHub account together
  - `$ git config --global user.name "Your name here"`
  - `$ git config --global user.email "your_email@example.com"`
- Unable to rebase
  - `git config pull.rebase true`
- When trying to push, you get the error `remote: Permission to .../.git denied to <username>.`
  - Check this link to update your credentials (macOS): https://docs.github.com/en/get-started/getting-started-with-git/updating-credentials-from-the-macos-keychain
     - Delete any old credentials
  - Create a new security token: Click your profile picture on top right --> Settings --> Developer Settings --> Personal Access Tokens --> Fine-grained tokens. Generate a new token with "All Repositories" selected, and give yourself all repostory + account permissions. Save this token.
  - Try pushing again, it should prompt you for username and password. Paste the token for the prompted password.

- If you need help at any time, feel free to let us know! We'll try and help you resolve the error.
