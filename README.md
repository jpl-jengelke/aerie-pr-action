# Aerie Pull Request Action

A simple Github action to automatically assign assignees and reviewers to Pull Requests (PRs).

# Usage
```yaml
name: "Handle PR Logic"
on:
  pull_request
jobs:
  pr_logic:
  steps:
    - uses: nasa-ammos/aerie-pr-action@main
      with:
        numReviewers: 1
```
will automatically assign the opener of a PR as the assignee, and randomly assign 1 reviewer from the CODEOWNERs list in `./github/CODEOWNERS`