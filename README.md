# Gestion de Fichiers Musicaux MP3 et FLAC

Ce projet consiste en la création d'une application en Python permettant de gérer et manipuler des fichiers musicaux au format MP3 et FLAC, en exploitant leurs métadonnées. Le projet prend en charge les modes console (CLI) et interface graphique (GUI) pour permettre l'exploration de dossiers musicaux, l'affichage des métadonnées, et la gestion de playlists.

## Description

### Script 1 : CLI

Le script Cli permet de gérer et manipuler des fichiers audio MP3 et FLAC . Il offre une série de fonctionnalités pour l'extraction, l'affichage et la modification des métadonnées (tags) des fichiers, ainsi que la gestion de playlists.

Fonctionnalités du script :
- Extraction et affichage des métadonnées des fichiers MP3 (ID3) et FLAC (Vorbis comment).
- Exploration récursive des dossiers pour identifier les fichiers MP3/FLAC.
- Création de playlists au format XSPF.
- Possibilité de modifier et sauvegarder les métadonnées (tags) d'une chanson.

### Script 2 : GUI

Le mode GUI offre une interface visuelle permettant aux utilisateurs d'explorer, d'afficher et de modifier leurs fichiers audio MP3 et FLAC, tout en proposant des fonctionnalités supplémentaires, telles que l'intégration avec l'API Spotify.

Le script gui.py sert de point d'entrée principal pour le mode GUI, gérant la conception et l'affichage de l'interface visuelle. Son rôle est principalement de fournir une interface utilisateur intuitive pour explorer, afficher et modifier les fichiers audio MP3 et FLAC. En plus de cela, il offre des fonctionnalités avancées telles que l'intégration avec l'API Spotify pour la recherche d'albums et de chansons.

Toute la logique sous-jacente, y compris les fonctionnalités liées à l'extraction et la modification des métadonnées, la gestion des playlists, ainsi que l'interaction avec l'API Spotify, est importée à partir des modules Python situés dans le répertoire library. Ces modules gèrent le traitement des fichiers et l'accès aux services externes, tandis que gui.py se concentre sur l'expérience utilisateur et l'interaction avec ces fonctionnalités.

Fonctionnalités du script :
 
#### MUSIC MANAGER : 
- Extraction et affichage des métadonnées des fichiers MP3 et FLAC.
- Exploration des dossiers pour identifier les fichiers MP3/FLAC.
- Création d'une playlist pour un repertoire donne ou bien une playlist personnalisé au format XSPF.
- Possibilité de lire une chanson sélectionnée avec la fonction de navigation pour passer à la piste suivante ou précédente.

#### SPOTIFY :
- Recherche et Affichage des informations detaillées d’un album via une API.
- Recherche d'une chanson, affichage de ses métadonnées, avec possibilité de lecture.


## Installation

### Prérequis

- Python 3.x
- Bibliothèques Python requises 

```
pip install mutagen
pip install pygame
pip install PyQt5
pip install ffpyplayer
pip install spotipy
pip install qfluentwidgets

```


## Utilisation

### Mode CLI 

- Exécutez les commandes suivantes pour explorer des fichiers ou dossiers :

#### Afficher l'aide :
``` python modecli.py -h ```

#### Explorer un dossier  :
``` python modecli.py -d "chemin_du_repertoire" ```

#### Analyser un fichier MP3 ou FLAC spécifique :
``` python modecli.py -f fichier.mp3 ```

#### Sauvegarder la playlist générée dans un fichier :
``` python modecli.py -d "chemin_du_repertoire" -o playlist.xspf ```

#### Modification des metadonées d'un fichier :
``` python modecli.py --file music.mp3 --set-tags Title="New Title" Artist="New Artist" Album="New Album"  ```      

####  Lecture des fichiers musicaux  :
``` python modecli.py ```


### Mode GUI

- Exécutez la commande suivante pour lancer le mode graphique :

```python gui.py ```




## Auteur
- **Nom et Prénoms :** 
  Aourane Lyna Ines
- **Université :** CY Cergy Paris Université
- **Date :** 03-12-2024
