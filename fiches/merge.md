# `git <merge>` en 10 lignes

**À quoi ça sert** : Permet de fusionner deux commits

**La forme courante** : `git <merge> [-m <msg>] <branche>`


**Un exemple qu'on peut taper** (testé dans `git-carnet`) :
```bash
`<<<<<<< HEAD
# Crêpes au rhum
=======
# Crêpes
>>>>>>> parent of 202133b (Crepes a la biere)

- 250 g de farine
- 3 œufs
- 50 cl de lait
<<<<<<< HEAD
- 1 cuillère a soupe de rhum
=======
>>>>>>> parent of 202133b (Crepes a la biere)

Cuisson : 3 min par face, à feu vif.

Servir chaud, avec du sucre.
`

```

**Ce que ça affiche / ce que ça change** :  crée un commit à deux parents.

**Le piège** ⚠️ : Si un même fichier est modifié dans deux branches différentes, il faut en général régler les conflits manuellement. Ne pas commit un merge en conflit.

**Commande voisine** : `git merge --abort` – Permet d'annuler un merge en cours

Auteur : Emmanuel Ghesquier (`@26Emmanuel`)
