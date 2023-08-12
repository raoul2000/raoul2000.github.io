---
title: "filter"
date: 2023-06-11T12:28:31+02:00
draft: false
cover:
    image: "images/cover.png"
    alt: "filter"
    hidden: true
tags:
  - clojure    
  - animation    
---

![filter](./images/filter.gif)

```
(filter f coll)
```
The `filter`  function takes 2 arguments : 
- `f`: a function that takes one argument *x* and returns TRUE or FALSE [^1] .
- `coll`: a *collection* of items

`filter` returns a sequence of items from the *collection* for which *f* returns TRUE (it's the *opposite* of [remove](/posts/remove)).

> In the above animation, *f* returns TRUE when the item is a triangle or when it is blue.

[filter](https://clojuredocs.org/clojure.core/filter)

[^1]: such function is called a *predicate*