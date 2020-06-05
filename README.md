# Enrichissement-des-donnees-COVID-19-Sante-Publique-France

***Nouvelle version !!!  Ajout d'analyses relatives au déconfinement***

**Données actualisées le 04/06/2020  pour les trois jeux de données** *(sauf pour données relatives aux tests de dépistage)*

**site de téléchargement et d'information** : [https://www.fcafcadata.net/](https://www.fcafcadata.net/)

La réutilisation concerne les trois jeux données publiés sur le site datagouv.fr. par Santé Publique France:

Données des urgences hospitalières et de SOS médecins relatives à l'épidémie de COVID-19
Données hospitalières relatives à l'épidémie de COVID-19
Données relatives aux tests de dépistage de COVID-19 réalisés en laboratoire de ville

Mon objectif est de faciliter la prise en main des data par des profils de type statisticiens ou data scientist.
Il semble concevable que l’on puisse ajouter de nouvelles visualisations, des nouveaux indicateurs, en complément à ceux présentés chaque soir par le Pr Salomon.
Des projections, ratios, corrélations éventuellement cachées. « Mesurer pour comprendre » (devise de l’INSEE)

Les trois jeux sont à la granularité du département. Le référentiel d'enrichissement est donc identique pour les trois. 
Il comporte 17 colonnes qui précèdent celles des données : 
Préfecture du dpt, indication de préf. de région, latitude et longitude (pour carto), superficie, population INSEE, par tranches d'âge, etc...

J’ai démarré la réalisation d’une série de tableaux de bord, avec l’outil libre et open source Apache Superset qui représente une alternative crédible au « poids lourd » du secteur : Tableau.
[https://github.com/apache/incubator-superset](https://github.com/apache/incubator-superset)
Malheureusement, pour l’instant, je ne dispose pas d’une instance dimensionnée pour proposer un accès public à Superset.
Dans l’attente, je publie des copies d’écran. Trois thèmes sont abordés, dont l'évaluation du déconfinement :

Thème 1 : Evaluation du déconfinement (nouvelle version)
J’ai revu ma copie. Pour calculer le % d’évolution, je comparais la donnée du jour, avec celle publiée le premier jour du déconfinement.
J’ai découvert dans la dernière version d’Apache Superset qu’un certain nombre de courbes précalculée était disponibles, dont « mean », la moyenne glissante ou mobile.
Pour proposer une vision plus réaliste de l’évolution, c’est ce modèle de courbe qui est utilisé pour afficher la série de valeur.
J’ai remplacé la valeur du 11/05 par la moyenne des 10 jours précédents.

**Depuis le 28/05, le Val d’Oise apparaît en rouge dans le dashboard de l’Île-de-France. 
C’est aussi le cas de plusieurs départements, situés dans d’autres régions. A surveiller d’ici la fin de la phase 2. 
04/06 : La région Bretagne passe en « rouge » suite aux mauvais chiffres du Morbihan : +138.7%**

"*C'est dans l'angoisse que l'homme prend conscience de sa liberté.*" (Jean-Paul Sartre)
