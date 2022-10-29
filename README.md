# ProjetDataViz
Projet de visualisation des données en Python en L3 à l'université Sorbonne Paris Nord.
Nous avons décidé  de mener une étude sur un fichier nomme data que nous avons scinder en 4. Ce fichier contient un nombre de 4877 lignes.


## Présentation de la problématique
Nous allons essayer de montrer l'évolution de la pollution aérienne sur la période 2012-2017

### Description des fichiers :
lien de téléchargement : https://www.data.gouv.fr/fr/datasets/r/e5626b68-4615-41cb-90d0-1f825d520bd9

Ce jeu de données contient des informations sur les principaux polluants, notamment les particules en suspension (PM10, PM2,5) et le dioxyde d'azote (NO2) en microgramme par mètre cube (µg/m3) de moyenne journalière annuelle.

PM10 PM2,5: Les particules en suspension (notées « PM » en anglais pour « Particulate matter ») sont d’une manière générale les fines particules solides portées par l’eau ou solides et/ou liquides portées par l’air (Wikipédia). Chaque fichier comporte trois catégories de variables :

Les variables descriptives de l'établissement ; les variables rapportant les niveaux d'exposition ; une variable "geometry" correspondant à l'adresse géolocalisée de chaque établissement. Les variables descriptives des établissements sont des chaînes de caractères.

ID : l'identifiant unique de la crèche ou de l'école ; nom : le nom usuel de l'établissement dans les fichiers de référence ; CP : le code postal de l'établissement ; ville : la ville suivant la nomenclature de l'Insee ; type : la catégorie d'établissement (crèche, primaire ou secondaire). Les variables correspondant aux niveaux d'exposition suivent la nomenclature suivante : "polluant_AAAA", AAAA figurant l'année civile sur 4 chiffres. Leurs valeurs numériques sont exprimées en microgrammes par mètre cube en moyenne journalière annuelle.

### Normes de qualité de l’air en France :
Objectif de qualité : un niveau de concentration de substances polluantes dans l’atmosphère à atteindre à long terme, sauf lorsque cela n’est pas réalisable par des mesures proportionnées, afin d’assurer une protection efficace de la santé humaine et de l'environnement dans son ensemble
Valeur limite : un niveau de concentration de substances polluantes dans l’atmosphère fixé sur la base des connaissances scientifiques à ne pas dépasser dans le but d’éviter, de prévenir ou de réduire les effets nocifs de ces substances sur la santé humaine ou sur l'environnement dans son ensemble
pour le DIOXYDE d’AZOTE (NO2)

Objectif de qualité : 40 µg/m³ en moyenne annuelle
Valeurs limites pour la protection de la santé humaine : 40 µg/m³ en moyenne annuelle
pour les PARTICULES PM10

Objectif de qualité : 30 µg/m³
Valeurs limites pour la protection de la santé humaine : 40 µg/m³ en moyenne annuelle
pour les PARTICULES PM2,5

Objectif de qualité : 10 µg/m³ en moyenne annuelle
Valeurs limites pour la protection de la santé humaine 25 µg/m³ en moyenne annuelle
Source d'information : https://www.airparif.asso.fr/la-reglementation-en-france

## Information sur geopandas
GeoPandas étend les types de données utilisés par pandas pour permettre des opérations spatiales sur des types géométriques. Les opérations géométriques sont effectuées par shapely

## Installation de geopandas :

- Méthode 1 :

documentation geopandas sur le lien https://geopandas.org/getting_started/install.html
conda install geopandas
- Méthode 2 :

télécharger : Fiona, Pyproj, Shapely, GDAL and Geopandas wheels sur le lien : https://www.lfd.uci.edu/~gohlke/pythonlibs/

Installer les fichiers.whl manuellement avec pip sur Anaconda Prompt comme suit :

pip install *.whl en l'ordre suivant : GDAL, Pyproj, Fiona, Shapely et Geopandas

## Information sur mapclassify
mapclassify implémente une famille de schémas de classification pour les cartes choroplèthes. Il se concentre sur la détermination du nombre de classes et sur l'affectation des observations à ces classes.

Pour installer, taper la commande sur anaconda prompt :

pip install mapclassify

## Information sur les cartes
Ce jeu de données provient d'un service public certifié.

Découpage départemental de la région Île-de-France.

Télécharger et décompressé les fichiers geoflare des départements d'Île-de-France pour pouvoir les utiliser comme une carte de base.

https://www.data.gouv.fr/fr/datasets/r/2dedae24-eb12-4a92-803d-7ceddf08baf8
