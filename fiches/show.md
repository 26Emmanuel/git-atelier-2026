# `git show` en 10 lignes

**À quoi ça sert** : afficher un commit, son auteur, sa date, son message, et ce qu'il a changé.

**La forme courante** : `git show <commit>` (sans argument : `HEAD`, le dernier commit)

**Un exemple qu'on peut taper** (testé dans `git-carnet`) :

```bash
git show a9bfd1f                   # le commit entier : en-tête, message, diff
git show HEAD~1 --stat             # seulement la liste des fichiers touchés
git show main:recettes/tarte.md    # un fichier tel qu'il est dans main, sans changer de branche
```

**Ce que ça affiche / ce que ça change** : l'en-tête du commit, puis son diff. Rien n'est modifié : `show` ne fait que lire.

**Le piège** ⚠️ : dans `<commit>:<fichier>`, le chemin part de la racine du dépôt, pas du dossier courant ; depuis `recettes/`, écrivez `main:./tarte.md`.

**Commande voisine** : `git log -p` – le même affichage, mais pour toute une série de commits.

Auteur : Raphael Prasquier (`@raphaelpra`)
