# Exercices

---

## Modalités

1. Le but du jeu est que chacun travail sur une branche dédiée sur les mêmes fichiers donc nommez vos fichiers et dossiers à l'identique. Par contre le contenu doit être différent donc vous ne devez pas vous concertez pour avoir les mêmes recettes.

2. Il doit toujours y avoir un écran partagé par binôme sur TEAMS.
3. Je suis en soutien, n'hésitez pas à m'appeler **EN PREMIER** en cas de blocage, incompréhension, application etc. avant d'aller voir sur Internet.

3. Un temps est donné pour la réalisation de chaque partie avant de procéder à la correction et enchainer sur la partie suivante.

---

## Ressources

- Cours dans son intégralité (PDF)
- Le formateur
- La terminologie du cours (PDF)
- Recap des commandes (REPO GITHUB du Cours)
- Git cheat sheet sur (SLACK)

---

## Organisation

Pour les exercices en binôme :

1. Au départ créez un seul dépôt distant pour 2 depuis UN SEUL compte GitHub.
2. Celui qui a créé le dépôt, invite l'autre binôme à travailler sur ce dépôt depuis `settings > collaborators > add peole` en indiquant son adresse e-mail.

![](../3-tp/img/jpg/access.jpg)

3. Chacun travail sur une branche dédiée, nommez vos branches en suivant ce pattern (modèle) `feature/votreprenom/part1` pour la partie 1, ensuite  pour la suite , suivre les instructions de l'énoncé.
**Attention vous devez toujours créer vos branches à partir de la branche principale `main` ou `master`**. main ou master on parle de la même chose, la convention a juste changée entre temps avant la branche principale était nommée master, aujourd'hui c'est main.
Pour créer une nouvelle branche :
- S'assurer d'être bien sur la branche main ou master à l'aide de la commande git branch qui doit afficher un * sur la branche courante
- Ensuite exécutez la commande suivante : `git checkout -b feature/votrePrenom/partX`en remplaçant X part le numéro de la partie.
4. Ensuite chacun travail sur l'exercice depuis sa branche en suivant l'énoncé.
5. Lorsque vous avez fini vous devez faire un commit
- Pour faire un commit vous devez d'abord ajouter les fichiers concernés dans l'index ou stage à l'aide de la commande `git add fichier dossiers`
- Ensuite, il faut ajouter le message de commit qui explique les raisons de vos modifications/ajouts/suppressions etc cf. appuyez-vous sur les conventions de nommage d'[Angular](https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines), tous les commits doivent être en ANGLAIS
6. Vous devez envoyer vos modifications depuis votre branche en local vers votre branche distant à l'aide de la commande `git push -u  origin feature/votrePrenom/partX`

---

## Enoncés des exercices

---

### Partie 1

1. Récupérez le dépôt distant en local.
- `git clone url`
2. Créez et placez-vous sur une nouvelle branche nommée dédiée à cette partie et à votre prénom
- S'assurer d'être sur la main ou master cf. explications ci-dessus point 3 du chapitre `Organisation`
3. Créez un répertoire (dossier) sandwich. 
4. Créez un fichier à l’intérieur du répertoire sandwich nommé burger.md qui contient la liste des ingrédients qui compose un burger (un ingrédient par ligne).
Ajoutez une photo, pour ajouter une photo depuis un fichier markdown (.md), vous devez écrire `![n'importe quoi ici pour indiquer le nom](chemin_relatif_de_ce_fichier/vers_le_fichier_de_l'image_en_respectant_les_dossiers_ou_sous_dossiers/monimage.jpg)`

Exemple rendu final : 

Steak

Salade

Tomate

Cornichon

Fromage

![img](https://www.vegetalsquare.fr/1017-large_default/fish-filets-26kg-moving-mountains.jpg)

---

## Partie 2

1. Créez quelques autres sandwichs (hot_dog.md et jambon_beurre.md), un nouveau sandwich = une nouvelle branche.
2. Modifiez le contenu de burger.md .
3. Regardez l’état de votre dépôt.
- à l'aide de la commande `git status`
4. Ajoutez d'autres photos.
5. Regardez l’historique de vos commits.
- `git log` pour voir toutes les options possibles `git log --help`.
6. Effectuez au moins 5 modifications au total sur l’ensemble de vos fichiers. Chaque modification doit donner lieu à un commit. 5 modifications = 5 commits différents.

---

## Partie 3

1. Depuis GitHub, un collaborateur modifie le contenu de burger.md et fait un commit .

2. En local, faites une modification sur la même ou les mêmes lignes puis faites un commit.

3. En local, sur la même branche, récupérez les modifications effectuées en ligne.
- `git fetch`

4. Résolvez les conflits et commitez.
