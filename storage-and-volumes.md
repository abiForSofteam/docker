###### [Accueil](README.md)
### Storage and Volumes

###### Les fichiers créés dans un conteneur sont stockés par défaut dans une couche inscriptible de ce conteneur.
###### Les données du conteneur ne seraient donc plus disponibles si ce dernier venait à être supprimé, ce qui pourrait être problématique  si ces données étaient nécessaires au bon fonctionnement d'autres processus.
###### L'utilisation des volumes est la solution à cette situation.

###### De plus, l'écriture dans la couche inscriptible du conteneur requiert le pilote de stockage pour la gestion du système de fichier, ce qui réduit les performances du processus d'écriture, alors qu'en utilisant les volumes, l'écriture se fait directement dans le système de fichier de l'hôte.
###### Ainsi, les données du volume persistent même si le conteneur n'existe plus. 

#### Mise en évidence de données non persistantes
Etat des lieux avant la création de conteneur
![image](https://github.com/abiForSofteam/docker/assets/56606441/a10ccc40-e65d-48b4-8b5f-5fd4de6cc0bb)


Le pilote de stockage par défaut est overlay2
![image](https://github.com/abiForSofteam/docker/assets/56606441/d2d4fbc3-502f-4033-a1d1-a3d887375609)

