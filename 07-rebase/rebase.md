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
