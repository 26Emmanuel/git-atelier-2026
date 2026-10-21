# Atelier Git – 22 octobre 2026

Dépôt de classe du cours « Git » (Mines Paris, 2026). Chacun y contribue une fiche
« une commande git en 10 lignes », par une branche, une pull request et la review d'un camarade.
Les consignes pas à pas sont sur le site du cours : <https://git.mines.prasquier.dev> (séance GIT2, atelier).

## La règle du jeu

1. Vous forkez ce dépôt, vous clonez votre fork, vous ajoutez ce dépôt comme `upstream`.
2. Une branche `fiche/<commande>` par fiche, créée depuis `main`.
3. La fiche se rédige à partir de [`fiches/_modele.md`](fiches/_modele.md) et s'appelle `fiches/<commande>.md`.
4. Chaque PR modifie aussi [`SOMMAIRE.md`](SOMMAIRE.md) : une ligne à la fin de la liste. Oui, tout le monde ajoute sa ligne au même endroit.
5. `main` est protégée : on y entre par PR, relue par un camarade, mergée par le prof. Pas de push direct, pas de force-push.
6. Vous mettez votre branche à jour par `git fetch upstream && git merge upstream/main`, puis `git push`.

## Les commandes à documenter

Premier arrivé, premier servi : la branche poussée fait foi. `show` est pris : c'est la fiche d'exemple, [`fiches/show.md`](fiches/show.md). Une commande par fiche, un élève par commande
pour la première fiche ; pour la seconde, prenez ce qui reste.

`add -p` · `bisect` · `blame` · `branch` · `cherry-pick` · `clean` · `clone` · `commit --amend` · `diff` ·
`fetch` · `grep` · `log` (options utiles) · `merge` · `mv` · `pull` · `push` · `rebase` · `rebase -i` ·
`reflog` · `remote` · `reset` · `restore` · `revert` · `rm` · `shortlog` · `stash` · `status` ·
`switch` · `tag` · `worktree` · `.gitignore` · `config` (alias, editor)

## Ce qui est attendu d'une fiche

Dix lignes, pas un roman : à quoi sert la commande, sa forme la plus courante, un exemple qu'on peut taper,
un piège, une commande voisine. Testez l'exemple avant de l'écrire.
