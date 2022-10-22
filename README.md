# ProjetDataViz
Projet de visualisation des données en Python à L3 a l'université Sorbonne Paris Nord
Nous avons decide de mener une etude sur un fichier nomme data que nous avons scincer en 4. Ce fichier contient un nombre de 4877 ligne.


## Présentation de la problématique
On va essayer de montrer l'évolution de la pollution aérienne sur la période 2012-2017

### Description des fichiers :
lien de téléchargement: https://www.data.gouv.fr/fr/datasets/r/e5626b68-4615-41cb-90d0-1f825d520bd9

Ce jeu de données contient des informations sur les principaux polluants notamment les particules en suspension (PM10, PM2,5) et le dioxyde d'azote (NO2) en microgramme par mètre cube (µg/m3) de moyenne journalière annuelle.

PM10 PM2,5: Les particules en suspension (notées « PM » en anglais pour « Particulate matter ») sont d’une manière générale les fines particules solides portées par l’eau ou solides et/ou liquides portées par l’air (Wikipédia). Chaque fichier comporte trois catégories de variables :

les variables descriptives de l'établissement ; les variables rapportant les niveaux d'exposition ; une variable "geometry" correspondant à l'adresse géolocalisée de chaque établissement. Les variables descriptives des établissements sont des chaînes de caractères.

ID : l'identifiant unique de la crèche ou de l'école ; nom : le nom usuel de l'établissement dans les fichiers de référence ; CP : le code postal de l'établissement ; ville : la ville suivant la nomenclature de l'Insee ; type : la catégorie d'établissement (crèche, primaire ou secondaire). Les variables correspondant aux niveaux d'exposition suivent la nomenclature suivante : "polluant_AAAA", AAAA figurant l'année civile sur 4 chiffres. Leurs valeurs numériques sont exprimées en microgrammes par mètre cube en moyenne journalière annuelle.
