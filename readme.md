#### Présentation NetBox
Dans notre projet de fin d'étude, nous avons décider de mettre en place netbox.

###
Le contexte 

Nous sommes une ESN, LYMA Consulting, et nous avons pour projet la refonte complète de l'infrastruture d'un client : AquaLab

Ce client possède deux sites, un sur Bordeaux et l'autre à Pau.


NetBox est un outil open-source de gestion des infrastructures qui permet aux équipes informatiques de suivre et de gérer efficacement , les équipements réseau, les serveurs, les adressages IP les racks et autres éléments de leur infrastructure. fournit une base de données centralisée pour stocker des informations sur les ressources réseau et une interface web pour visualiser et gérer ces ressources.


```
git clone -b release https://github.com/netbox-community/netbox-docker.git
cd netbox-docker
```

Ensuite, il faut ajouter la configuration suivante dans le fichier docker-compose.override.yml

docker-compose_override_yml.png

Puis tapez les commandes suivantes : 
```
docker compose pull
docker compose up
```