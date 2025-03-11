Un développeur doit maîtriser plusieurs scénarios courants avec Git pour travailler efficacement en équipe et gérer son code proprement. Voici les plus
importants :

📌 Scénarios de base

- Initialiser un dépôt (`git init`)
- Cloner un dépôt distant (`git clone <repo_url>`)
- Faire un commit (`git add . && git commit -m "Message"`)
- Pousser des modifications vers un dépôt distant (`git push origin <branch>`)
- Récupérer les modifications depuis un dépôt distant
  (`git pull origin <branch>`)

🔄 Gestion des branches

- Créer une nouvelle branche (`git checkout -b feature-x`)
- Basculer entre les branches (`git checkout main`)
- Fusionner une branche dans une autre (`git merge feature-x`)
- Supprimer une branche locale (`git branch -d feature-x`)
- Supprimer une branche distante (`git push origin --delete feature-x`)

🤝 Collaboration et résolution de conflits

- Mettre à jour sa branche avec la branche principale
  (`git pull origin main --rebase`)
- Résoudre un conflit de fusion (éditer les fichiers conflictuels, `git add`,
  `git commit`)
- Rebase une branche sur une autre (`git rebase main`)
- Annuler un rebase en cours (`git rebase --abort`)
- Revenir à un état précédent après une erreur (`git reset --hard HEAD~1` ou
  `git reflog`)

🛠 Révisions et corrections

- Voir l'historique des commits (`git log --oneline --graph --all`)
- Voir les différences entre commits ou branches (`git diff HEAD`)
- Modifier le dernier commit (`git commit --amend`)
- Créer un commit intermédiaire sans toucher à l'index (`git stash` et
  `git stash pop`)
- Annuler un commit sans supprimer les fichiers (git reset --soft HEAD~1)

🚑 Gestion des erreurs et récupération

- Annuler un commit déjà poussé (git revert <commit_hash>)
- Retrouver un fichier supprimé (git checkout -- <file>)
- Revenir à une version précédente du code (git checkout <commit_hash> --
  <file>)
- Annuler tous les changements non commités (git reset --hard)
- Annuler des modifications locales d'un fichier spécifique (git checkout --
  <file>)

🏎 Optimisation et bonnes pratiques

- Squash plusieurs commits en un seul (`git rebase -i HEAD~3`)
- Travailler avec des tags pour marquer des versions (git tag v1.0 && git push
  origin v1.0)
- Nettoyer l’historique des branches locales obsolètes (git branch --merged |
  grep -v '\*' | xargs git branch -d)
- Gérer des sous-modules Git (git submodule add <repo_url> <path>)
- Utiliser des hooks pour automatiser des tâches (.git/hooks/pre-commit par
  exemple)
