---
title: Open all files from a specific Git Commit in Vim
date: 2019-09-01
published: true
tags: ['Git']
series: false
cover_image: ./images/alexandr-podvalny-220262-unsplash.jpg
canonical_url: false
description: I occasionally find myself needing to open all files from a specific Git commit. This is easy to do with Vim!

---

I occasionally find myself needing to open all files from a specific Git commit. I use vim as my editor.

Soooo....

I created a little alias to get all the names of files modified in the specific commit and open them all in vim:

```
function vcommit(){
    vim $(git diff-tree --no-commit-id --name-only -r $1)
}
```
