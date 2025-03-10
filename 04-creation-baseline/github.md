# Créer une baseline github

- Avoir un compte github
- Etre connecté
- Creer un repo sous github

Les 3 commandes suivantes font :

- créer une reference de repository distant sur lequel on peut récupérer ou
  livrer du code.
- changer le nom de la branche principale en `master` (peut être la branche
  s'appelle déjà `master` et dans ce cas la commande est inutile)
- délivrer l'historique des commits de la branche `master`.

```
git remote add origin https://github.com/jlg-formation/git-manual.git
git branch -M master
git push -u origin master
```
