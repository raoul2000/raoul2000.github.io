---
title: "take-while"
date: 2023-09-09T13:18:07+02:00
draft: false
cover:
    image: "images/cover.png"
    alt: "take-while"
    hidden: true
tags:
  - clojure    
  - animation      
---

![filter](./images/take-while.gif)

```clojure
(take-while f coll)
```

La fonction `take-while` accepte 2 arguments : 
- `f`: une fonction qui prend un argument *x* et qui renvoie VRAI ou FAUX.
- `coll`: une *collection* d'éléments

`take-while` commence par le premier élément de la *collection* et retourne la séquence de tous les éléments **successifs**  pour lequels *f* renvoie VRAI. Aussitôt que *f* renvoie FAUX, `take-while` se termine et ne traite donc pas les éléments qui pourraient éventuellement suivre.

Contraitement à la fonction  [`filter`](../filter), `take-while` ne parcours pas tous les éléments de la *collection*.


> Dans l'animation ci-dessus, *f* renvoie VRAI lorsque l'élément est de couleur verte. Le troisième élément (rond bleu) vient interrompre le parcours de la collection : le dernier élément bien que de couleur verte n'est pas renvoyé par `take-while`.

[take-while](https://clojuredocs.org/clojure.core/take-while)