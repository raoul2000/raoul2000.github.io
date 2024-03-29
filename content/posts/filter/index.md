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

```clojure
(filter f coll)
```
La fonction `filter` accepte 2 arguments : 
- `f`: une fonction qui prend un argument *x* et qui renvoie VRAI ou FAUX [^1]
- `coll`: une *collection* d'éléments

`filter` retourne une séquence composée de tous les éléments de la *collection* pour lesquels *f* renvoie VRAI (c'est l'*inverse* de [remove](/posts/remove)).

> Dans l'animation ci-dessus, *f* renvoie VRAI lorsque l'élément est un triangle ou lorsqu'il est de couleur bleu.

[filter](https://clojuredocs.org/clojure.core/filter)

[^1]: une telle fonction est appellée un *prédicat*.




