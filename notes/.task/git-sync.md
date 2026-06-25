---
title: Git Sync
type: script
created: 2026-06-25T10:22:27+07:00
---

## Sync started

2026-06-25 10:22:27

```text
auto-sync: start 2026-06-25T10:22:27+07:00

$ git config --local credential.helper store --file=/data/healing.cred
-> ok


$ git config --local --get user.name
healing
-> ok


$ git config --local --get user.email
healing@gwiki.org
-> ok


$ git remote get-url origin
https://github.com/senomas/healing-wiki.git
-> ok


$ git rev-parse --verify HEAD
21b06973b7d664ee57d3dd9e74632d3ab5c74230
-> ok


$ git remote
origin
-> ok


$ git ls-remote --symref origin HEAD
fatal: unable to access 'https://github.com/senomas/healing-wiki.git/': Could not resolve host: github.com
-> error: exit status 128


$ git show-ref --verify refs/heads/master
-> ok

auto-sync: remote HEAD missing; skip fetch master

$ git checkout master
Already on 'master'
M	notes/.task/git-sync.md
Your branch is ahead of 'origin/master' by 135 commits.
  (use "git push" to publish your local commits)
-> ok


$ git add .
