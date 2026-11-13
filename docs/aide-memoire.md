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


## Branches

| Commande      | Ce qu'elle fait                                     | Exemple                                   |
| --------      | ----------------------------------                  | -------------------------                 |
| `git branch`  | Liste les branches de mon projet                    | `git branch`                              |
| `git switch`  | Cree une nouvelle branch et se positione dessus     | `git switch -c ajout-section`             |
