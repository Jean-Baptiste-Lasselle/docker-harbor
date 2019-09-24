# docker-harbor
Merci à Marc Yalap pour m'avoir amené à m'intéresser au produit


# J'ai raison ?

Bon, j'ai déjà regardé un tuto et _installer et lancer `Harbor`_, c'est simple : 

* On télécharge la distribution sous forme de `*.tar.gz`, qu'on décompresse
* Il y a une phase de configuration dans laquelle ils génèrent les certificats en local, et création/édition de quelques autres ficheirs de configuration, et : bref, au final, les fichiers de configuration sont là où il faut, avec le contenu qu'il faut.
* Dderrière c'est très simple l'installation de `Harbor`  : 
```bash
sudo ./install.sh --with-clair
```
* Et on comprend tout de suite pourquoi le nivau 3 de support périmètre systèmes (d'une certaine grosse société), veut `Harbor` : pour avoir "directement le scanner de vulnérabilités" de dispo avec la solution de docker registry.
* La recette que j'ai examinée repose sur un `docker-compose.yml`. Maintenant es-ce que `Harbor` se déploie facilement dans `Kubernetes`, ça, il faut avoir la réponse au plus tôt. Des chances que oui.

