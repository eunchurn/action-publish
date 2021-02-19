# `action-publish`

A GitHub Action to push any local file changes, including new files, back to supplied branch name.

This action is useful to put *after* other actions that modify files in the local checkout
that you'd then like to persist back into the repository.

Usage:

```
- uses: eunchurn/action-publish@v1
  env:
    GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
    BRANCH_NAME: '' #optional defaults to master
    USER_NAME: '' #optional defaults to "Automated publisher"
    USER_EMAIL: '' #optional defaults to "actions@users.noreply.github.com"
```

## Acknowledgement

- Refered to `https://github.com/mikeal/publish-to-github-action`