###### [Accueil](README.md)
### Storage and Volumes

Les fichiers créés dans un conteneur sont stockés par défaut dans une couche inscriptible de ce conteneur.
Les données du conteneur ne seraient donc plus disponibles si ce dernier venait à être supprimé, ce qui pourrait être problématique si ces données étaient nécessaires au bon fonctionnement d'autres processus.
L'utilisation des volumes est la solution à cette situation.

Le pilote de stockage par défaut est overlay2
![image](https://github.com/abiForSofteam/docker/assets/56606441/d2d4fbc3-502f-4033-a1d1-a3d887375609)

