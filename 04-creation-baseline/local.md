# Créer une baseline locale

- Créer un repo bare sous son disque dur

```
mkdir server-local
cd server-local
mkdir git-manual
cd git manual
git init --bare
```

Un repo bare ne crée pas de dossier `.git`. Il crée les fichiers techniques de
git directement sous le dossier avec le nom du repo.

Les 3 commandes suivantes font :

- créer une reference de repository distant sur lequel on peut récupérer ou
  livrer du code.
- changer le nom de la branche principale en `master` (peut être la branche
  s'appelle déjà `master` et dans ce cas la commande est inutile)
- délivrer l'historique des commits de la branche `master`.

```
git remote add local "D:/___GIT/server-local/git-manual"
git push -u local master
```

Attention : l'option -u mémorise le remote de destination est la branche à
pousser/récupérer. La commande `git push` sans arguments est suffisante par la
suite.
