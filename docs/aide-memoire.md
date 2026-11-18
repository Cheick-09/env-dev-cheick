# Aide-mémoire du terminal Linux

## Se déplacer

| Commande | Ce qu'elle fait                        | Exemple    |
| -------- | -------------------------------------- | ---------- |
| `pwd`    | Affiche le dossier où je suis          | `pwd`      |
| `cd`     | Change de dossier                      | `cd ~/dev` |
| `cd ..`  | Remonte au dossier parent              | `cd ..`    |
| `cd ~`   | Retourne dans mon dossier personnel    | `cd ~`     |
| `ls`     | Liste les fichiers du dossier          | `ls`       |
| `ls -l`  | Liste détaillée (droits, taille, date) | `ls -l`    |
| `ls -a`  | Montre aussi les fichiers cachés       | `ls -a`    |

## Fichiers et dossiers

| Commande | Ce qu'elle fait                    | Exemple                   |
| -------- | ---------------------------------- | ------------------------- |
| `mkdir`  | Crée un dossier                    | `mkdir archives`          |
| `touch`  | Crée un fichier vide               | `touch a.txt`             |
| `cp`     | Copie un fichier                   | `cp a.txt b.txt`          |
| `cp -r`  | Copie un dossier                   | `cp -r projet projet2`    |
| `mv`     | Déplace ou renomme                 | `mv a.txt logs/`          |
| `rm`     | Supprime un fichier                | `rm a.txt`                |
| `rm -r`  | Supprime un dossier et son contenu | `rm -r archives`          |
| `rmdir`  | Supprime un dossier vide           | `rmdir vide`              |
| `echo`   | Affiche un texte                   | `echo "Bonjour"`          |
| `chmod`  | Change les droits d'un fichier     | `chmod a-w important.txt` |

## Lire et chercher

| Commande   | Ce qu'elle fait                                 |Exemple                 |
| ---------- | ----------------------------------------------- |----------------------- |
| `cat`      | Affiche tout le fichier                         | `cat notes.txt`        |
| `less`     | Affiche page par page (`q` pour quitter)        | `less notes.txt`       |
| `head -n`  | Affiche les premières lignes                    | `head -n 5 notes.txt`  |
| `tail -n`  | Affiche les dernières lignes                    | `tail -n 5 notes.txt`  |
| `wc -l`    | Compte les lignes                               | `wc -l notes.txt`      |
| `grep`     | Affiche les lignes qui contiennent un mot       | `grep ERROR app.log`   |
| `grep -i`  | Pareil, sans tenir compte des majuscules        | `grep -i error app.log`|
| `grep -c`  | Compte les lignes qui contiennent le mot        | `grep -c ERROR app.log`|
| `grep -r`  | Cherche dans le dossier et ses sous-dossiers    | `grep -r "todo" .`     |
| `grep -rl` | Affiche seulement les noms des fichiers trouvés | `grep -r -l "todo" .`  |
| `find`     | Retrouver un fichier par son nom                | `find . -a "todo" `    |

## Enregistrer et enchaîner

| Symbole | Ce qu'il fait                                         | Exemple                        |
| ------- | ----------------------------------------------------- | --------------------           |
| `>`     | Écrit le résultat dans un fichier (efface le contenu) | `ls > liste.txt`               |
| `>>`    | Ajoute le résultat à la fin du fichier                | `echo "Idée 2" >> idee.txt'    |
| `\|`    | Donne le résultat d'une commande à la suivante        | `grep ERROR app.log \| wc -l`  |
| `sort`  | Trie les lignes par ordre alphabétique                | `sort liste.txt`               |


## Branches

| Commande      | Ce qu'elle fait                                     |     Exemple                   |
| --------      | -----------------------------------------------       -------------------------     |
| `git branch`  | Liste les branches de mon projet                    | `git branch                   |
| `git switch`  | Cree une nouvelle branch et se positione dessus     | `git switch -c  ajout-section |

## Astuce de yoann

| Commande           | Ce qu'elle fait                     | Exemple                    |
|---------------     |-----------------------------------  |----------------------      |
| `kill`             | Demande à un processus de s'arrêter | `kill 1234`                |