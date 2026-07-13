---
title: "PGP key & fingerprint"
date: 2026-07-13T21:00:26+02:00
tags: []
author: "Jean Letessier"
# author: ["Me", "You"] # multiple authors
showToc: true
TocOpen: false
draft: false
hidemeta: true
comments: false
description: "My PGP public key and fingerprint"
canonicalURL: "https://jeanl.is-a.dev/pgp/"
disableHLJS: true # to disable highlightjs
disableShare: false
hideSummary: false
searchHidden: false
ShowReadingTime: false
ShowBreadCrumbs: false
ShowPostNavLinks: true
ShowWordCount: true
ShowRssButtonInSectionTermList: true
UseHugoToc: true
editPost:
    URL: "https://github.com/Pixfri/pixfri.github.io/tree/main/content"
    Text: "Suggest Changes" # edit text
    appendFilePath: true # to append file path to Edit link
---

You can encrypt messages to me or verify my signatures using the public key below:
```text
E-Mail Address: jean.letessier@protonmail.com
Fingerprint: 3225 0A49 A51D 7F2C 9128 E93A 5483 B55C B19D 5D5B
Created: 2026-07-13
Expires: 2028-07-12
```

Download: [pgp-key.asc](/pgp-key.asc)

Use this key to:
- Encrypt messages / files to me.
- Verify my signed Git commits / signed messages.

To import:

```bash
curl -O https://jeanl.is-a.dev/pgp-key.asc
gpg --import pgp-key.asc
```

To verify the fingerprint matches after the import:

```bash
gpg --fingerprint jean.letessier@protonmail.com
```
