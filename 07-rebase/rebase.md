# Rebase

Conseil : Eviter de faire des **merges**, préférer faire des **rebase**.

Pourquoi ? Pour linéariser l'historique et le rendre ainsi plus lisible.

Par contre, éviter de changer l'historique d'une branche sur la baseline.

Pour faire un rebase d'une branche `truc` recemment créée à partir du master sur
laquelle on a fait des modifications de logiciel.

Se mettre sur la branche master.

```
git checkout master
```

Puis faire le merge façon rebase.

```
git rebase truc
```

## Scenario de 2 developpeurs qui bossent sur master

1. le dev 1 fait un fetch, un rebase, sa modification.

<<<<<<< HEAD
<<<<<<< HEAD
2. le dev 1 fait une modif dans son coin et commit.
=======
2. le dev 2 continue à développer et fait un commit sans push.
>>>>>>> 7b5f053 (dev: commit sans push)
=======
2. le dev 2 continue à développer et fait un commit sans push.
>>>>>>> 7b5f053 (dev: commit sans push)
