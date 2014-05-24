---
layout: default
title: The Zip in Python
comments: "yes"
disqus-id:
math: "yes"
last-major-revision-date:
license: "CC-BY"
tags: math
---

``` python
>>> x= (1,2,3)
>>> y=(4,5,6)
>>> tup=[x,y]
>>> tup
[(1, 2, 3), (4, 5, 6)]
>>> tup == zip(*zip(*tup))
```
