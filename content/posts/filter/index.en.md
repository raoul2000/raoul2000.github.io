---
title: "filter"
date: 2023-06-03T12:37:31+02:00
draft: true
---

![filter](./images/filter.gif)

```
(filter f coll)
```
The `filter`  function takes 2 arguments : 
- `f`: a function that takes one argument *x* and returns TRUE or FALSE [^1] .
- `coll`: a *collection* of items

`filter` returns a sequence of items from the *collection* for which *f* returns TRUE

> In the above animation, *f* returns TRUE when the item is a circle or when it is orange.

[filter](https://clojuredocs.org/clojure.core/filter)

[^1]: such function is called a *predicate*