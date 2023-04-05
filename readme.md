# Présentation NetBox
Dans notre projet de fin d'étude, nous avons décider de mettre en place netbox.

##
Le contexte 

Nous sommes une ESN, LYMA Consulting, et nous avons pour projet la refonte complète de l'infrastruture d'un client : AquaLab

Ce client possède deux sites, un sur Bordeaux et l'autre à Pau.

Voici les deux schéma réseau :

### Bordeaux
![image](https://github.com/hajimeeeee/Open-source_NETBOX/blob/main/screen/schema_bdx.PNG)


### Pau
![image](https://github.com/hajimeeeee/Open-source_NETBOX/blob/main/screen/schema_pau.PNG)


NetBox est un outil open-source de gestion des infrastructures qui permet aux équipes informatiques de suivre et de gérer efficacement , les équipements réseau, les serveurs, les adressages IP les racks et autres éléments de leur infrastructure. fournit une base de données centralisée pour stocker des informations sur les ressources réseau et une interface web pour visualiser et gérer ces ressources.

### Installation
```
git clone -b release https://github.com/netbox-community/netbox-docker.git
cd netbox-docker
```

Ensuite, il faut ajouter la configuration suivante dans le fichier docker-compose.override.yml :


![image](https://github.com/hajimeeeee/Open-source_NETBOX/blob/main/screen/docker-compose_override_yml.PNG)


docker-compose_override_yml.png

Puis tapez les commandes suivantes : 
```
docker compose pull
docker compose up
```
Nous pourrons donc accéder à l'interface Web de NetBox !

### Configuration

#### Création des sites

Nous allons ajouter les regions dans lesquels se trouvent nos sites :

![image](https://github.com/hajimeeeee/Open-source_NETBOX/blob/main/screen/regions.PNG)

Pour ensuite ajouter nos sites :

![image](https://github.com/hajimeeeee/Open-source_NETBOX/blob/main/screen/sites.PNG)


#### Baies & Equipements 

Nous pouvons ajouter nos baies, sachant que nous avons deux baies par sites, nous les avons ajouté tel que :
![image](https://github.com/hajimeeeee/Open-source_NETBOX/blob/main/screen/racks.PNG)


Nous pouvons aussi ajouter les équipements, de sorte à ce que nous ayons toutes les informations :

Constucteur, type d'équipement, modèle, nom, adresse IP, emplacement...

Nous avons ajouté nos équipements :
![image](https://github.com/hajimeeeee/Open-source_NETBOX/blob/main/screen/devices.PNG)


Pour nous en tant qu'ESN, il est important d'avoir un visuel sur les baies de nos clients et de leurs disposition.
Nous pouvons visualiser les baies de notre client AquaLab ainsi que la disposition des équipements dans ces baies.
