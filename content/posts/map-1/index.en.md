---
title: "map"
date: 2023-06-14T18:56:30+02:00
draft: true
cover:
    image: "images/map-1-cover.png"
    alt: "map"
    hidden: true
---

![filter](./images/map-1.gif)

```
(map f coll)
```

in this animation, the function `map` takes 2 arguments:
- `f`: a function that take one argument and returns one value
- `coll`: a *collection* of items

`map` returns a new list made of the result of *f* applied to each item from the *collection*. Consequently the list returned by `map` always contains the same number of items than the *collection* passed as argument.

> In the above animation, *f* paints into orange each item passed to it.


[map](https://clojuredocs.org/clojure.core/map)