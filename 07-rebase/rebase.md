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
2. le dev 1 fait une modif dans son coin et commit.
3. le dev 2 continue à développer et fait un commit sans push.
4. le dev 1 push.
5. le dev 2 push et cela presente un conflit.
6. le dev 2 va alors creer une branche avec son commit qu'il voulait pusher.
7. il pourra alors fetcher.
8. Il fait un rebase de sa branche.
9. Il peut alors pusher a nouveau.
10. Il rebase autant que necessaire.

## Mettre la config en pull rebase par defaut.

```
git config --global pull.rebase true
```
