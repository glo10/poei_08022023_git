# Partie 1

1. On clone le dépôt depuis notre dépôt distant
`git clone https://github.com/glo10/exercice_correction.git`


2. Chacun crée ses branches locales depuis la branche principale `main` ou `master`
- `git checkout -b feature/glodie/part1`
- `git checkout -b feature/xavier/part1`

5. Avant de commiter, au préalable, il faut ajouter les fichiers qui se trouvent par defaut sur le `working directory` dans le `stage (index)` à l'aide de la commande `git add`
- `git add sandwich` : ici on ajoute dans l'index tous les sous-dossiers et fichiers contenu dans sandwich, si vous devez ajouter un seul fichier précis, il faut indiquer son chémin relatif depuis votre emplacement dans le terminal
- `git commit -m 'feat: add burger'` : une fois qu'on a au moins un fichier dans le stage (index) = condition préalable, on peut commiter en indiquant la raison de nos modifications.
Les commits doivent être en anglais et en respectant les conventions de nommage de l'entreprise ou à defaut de la communauté.
6. Ici on envoie nos modifications vers le dépôt distant GitHub.
`git push -u origin feature/glodie/part1`
La première fois qu'une branche est créée en locale et qu'il n'existe pas en distant on a besoin de spécifier l'option `-u` pour créer cette branche en distance.
Une fois que la branche distante a été crée, pour les prochains, il n' y a pas besoin de spécifier la branche. On pourra directement écrire `git push`.
Git est suffisant intelligent pour détecter que vous êtes sur une branche X et d'envoyer les modifications à son homologue distant X.