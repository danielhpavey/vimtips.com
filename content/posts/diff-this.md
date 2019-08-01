---
title: Diff This with Vim
date: 2019-09-01
published: true
tags: ['Diff','Git']
canonical_url: false
cover_image: false
description: The :diffthis command allows us to compare two (or more) buffers that are open in an existing Vim session

---

The :diffthis command allows us to compare two (or more) buffers that are open in an existing Vim session. If we have two split windows containing buffers that we want to compare, then we can diff them by running:

````
:windo diffthis
````

We can turn diff mode off just as easily, by running:

````
:windo diffoff
````
