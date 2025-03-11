# Exercices

Voici une liste des exercices à savoir faire car ils correspondent à des
scénarios de la vraie vie dans Git.

## Rebase

2 développeurs travaillent en parallèle. L'historique doit rester linéaire.

Scenario :

1. les 2 developpeurs recuperent le projet en cours.
2. le dev A commit une modif et push.
3. le dev B commit une modif et push aussi. Un merge est demandé.
4. le dev B fait le merge (rebase) et push. L'historique est restée linéaire.

## Filter l'historique

1. un chef de projet parcours l'historique d'un projet.
2. il s'apercoit qu'un fichier ne devrait jamais rester dans l'historique car il
   contient des informations sensibles ou c'est un gros fichier.
3. le chef de projet filtre l'historique.
4. les développeurs recharge le nouvel historique.

## Toujours tester

1. le chef de projet en a marre des développeurs qui committent n'importe
   quoi...
   - code mal formatté
   - code mal linté
   - code qui ne build pas
   - test unitaire qui ne passent pas
2. Il veut que sur chaque push, un script soit joué est empéche le push si le
   script renvoie false ou sort en erreur.

## Deploiement automatique

1. des que le projet est buildé, il triggue un script de déploiement.

## Squasher des commits

1. Un chef de projet veut délivrer des commits à son client.
2. Pour des raisons de confidentialités il ne veut pas montrer tous les commits
   intermédiaires.
3. Il squash des commits.
