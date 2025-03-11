# Premier commit

Pour sauver ce qu'on a fait, on execute un commit. Voici comment faire :

Dans le répertoire git-manual

```
git add *
git commit -m "Mon premier commit"
```

## Prerequis

Il faut avoir un email et un nom de commit car un commit ne peut être anonyme.

```
git config --global user.name "Jean-Louis GUENEGO"
git config --global user.email jlguenego@gmail.com
```

## Deuxieme commit

```
git add *
git commit -m "Mon deuxieme commit"
```

## Commit

Un commit comprend :

- une arborescence de fichiers
- du texte caractérisant le descriptif, la date et l'auteur et le créateur du
  commit.
- la reference du commit précédent, lequel constitue l'historique par recursion,
  sauf si c'est un commit initial.

## Branche

- une branche est un pointeur sur un commit.
- Lorsqu'on dit qu'on fait un commit sur une branche, la branche pointe sur le
  nouveau commit, et ce nouveau commit déclare l'ancien commit comme commit
  précédent.

## Branche courante

Dans Git, on peut créér autant de branche que l'on souhaite. Git est toujours
réglé sur une branche courante.
