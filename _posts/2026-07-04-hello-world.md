---
title: "Hello, world"
categories: [meta]
---

First post. This blog is where I'll write about GDB and binutils internals,
the ongoing port of GNU binutils-gdb to the HPE NonStop Server, C++ on Linux
backends, and embedded / real-time work.

The site itself is a plain Jekyll setup on GitHub Pages. Adding a post is:

```sh
$EDITOR _posts/2026-07-10-my-new-post.md
git add _posts/2026-07-10-my-new-post.md
git commit -m "Post: my new post"
git push
```

No build step on my side — GitHub Pages renders it on push.
