# Fiche réseau

## Mes adresses IP

| Machine                | Adresse IP    | Privée ou publique ? | Comment la trouver                                |
| ---------------------- | ------------- | -------------------- | ------------------------------------------------- |
| Mon Ubuntu             |172.20.39.189  | privée               | `hostname -I`                                     |
| Mon ordinateur (Wi-Fi) | 172.16.50.83  | privée               | `ipconfig` (Windows) ou `ip a` (Linux)            |
| Ma connexion Internet  | (non publiée) | publique             | `curl ifconfig.me` (à ne pas publier)             |

> Une adresse privée commence par `10.`, `172.16.` à `172.31.` ou `192.168.`. Elle n'est visible que dans mon réseau local.

## Résultats du DNS

| Nom de domaine  | Adresse IP   | Commande                  |
| --------------- | ----------   | ------------------------- |
| `github.com`    |140.82.121.4  | `nslookup github.com`     |
| `wikipedia.org` |185.15.59.224 | `nslookup wikipedia.org`  |

> Ces adresses peuvent changer selon l'endroit et le moment : je note celles que mon `nslookup` m'a donné.

## Les outils réseau

| Commande           | Ce qu'elle fait                                                                 |
| -----------------  | ------------------------------------------------------------------------        |
| `hostname -I`      | Affiche l'adresse IP de mon Ubuntu                                              |
| `ip a`             | Liste les interfaces réseau et leurs adresses                                   |
| `ping -c 4 <nom>`  | Envoie 4 paquets à la machine pour tester si elle répond et en combien de temps |
| `nslookup <nom>`   | Interroge le DNS pour traduire un nom de domaine en adresse IP                  |
| `curl ifconfig.me` | Affiche l'adresse IP publique de ma connexion Internet                          |