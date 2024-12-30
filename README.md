# PHP et MySQL avec Docker

## Prérequis

- [Docker](https://docs.docker.com/install/)
- [Docker Compose](https://docs.docker.com/compose/install/)

## APPLICATION 
### Lancement de l'application
- **Cloner** le repos à l'aide *git clone @repos*
- **Se placer** au niveau d'arborescence du fichier *docker-compose up*

### Services fournies par l'application (fichier docker-compose.yml )

- **nginx** : Serveur HTTP exposé sur le port `8080`, utilisant une configuration personnalisée et les fichiers de `./code`.
- **php** : Exécute le code PHP des fichiers de `./code`.
- **mysql** : Base de données MySQL, persistante via le volume dbdata, exposée sur le port `3306` et accessible notament via `mySQLWorkbench`.
- **phpmyadmin** : Interface web pour MySQL, accessible sur le port `8081`.
- **[PURE-FTP](https://github.com/stilliard/docker-pure-ftpd/blob/master/README.md#example-usage-once-inside)** : Serveur FTP avec l'utilisateur `bob` et pass `12345`, partageant `./code` et exposant les ports `21` et `30000-30009`.


`Cette configuration est modifiable, il faudra modifier le fichier docker-compose.yml si besoin`.

## Travail demandé
- [Exercice de cours (serie 1)](https://drive.google.com/drive/folders/1Z1rfzunWnGNBq75whRLLoDzPM-z6OVgF?usp=sharing)
- [Exercices de cours (serie 2)](https://docs.google.com/presentation/d/1PG87x0raTYsk-iZmx32mN_CsQwRd094w0ocE8NHQmkE/edit?usp=sharing)
- [Salaire Median des Employés avec BDD mySQL](https://docs.google.com/presentation/d/1eMEw64LA3leFQgHyA_3WdMTsA3p8Xv7weeY8qaXls-o/edit?usp=sharing)
- [Salaire Median des Employés avec BDD mySQL avec Jointures](https://docs.google.com/presentation/d/13ExMTgjQdMjZPAwUS1Igpq48rKLUlJFjpdMPJBd6-1k/edit?usp=sharing)
