---
layout: post
title: "Hello World!"
date: 2014-02-06 18:39:04 +1100
comments: true
categories: python, quine
---
Welcome to this Octopress blog, yo.

Here's a Python [Quine](https://en.wikipedia.org/wiki/Quine_%28computing%29)

```python
#!/usr/bin/env python
x = """#!/usr/bin/env python
x = {0}
# These comments make up 40% of this quine.
print(x.format('"'*3 + x + '"'*3))"""
# These comments make up 40% of this quine.
print(x.format('"'*3 + x + '"'*3))
```

Mmmm, highlighting.
