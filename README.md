***Nouvelle version !!! (09/07) : Ajout d'analyses relatives au déconfinement depuis le 1er Juin***  

**Données hospitalières relatives à l'épidémie de COVID-19**
**Données des urgences hospitalières et de SOS médecins relatives à l'épidémie de COVID-19**
**Données relatives aux tests de dépistage de COVID-19 réalisés en laboratoire de ville** *(production interrompue par SPF depuis le 29/05)*  

**Données relatives aux résultats des tests virologiques COVID-19 (SI-DEP)** *(production récente)*

Données actualisées le **09/07/2020**  pour les quatre jeux de données *(sauf pour données relatives aux tests de dépistage)*

Mon objectif est de faciliter la prise en main des data par des profils de type statisticiens ou data scientist.
Il semble concevable que l’on puisse ajouter de nouvelles visualisations, des nouveaux indicateurs, en complément à ceux qui étaient présentés chaque soir par le Pr Salomon.
Des projections, ratios, corrélations éventuellement cachées. « Mesurer pour comprendre » (devise de l’INSEE)

Les quatre jeux sont à la granularité du département. Le référentiel d'enrichissement est donc identique pour les quatre.
Il comporte 17 colonnes qui précèdent celles des données : 
Préfecture du dpt, indication de préf. de région, latitude et longitude (pour carto), superficie, population INSEE, par tranches d'âge, etc...

J'ai créé un dépôt git : [https://github.com/fcafca/Enrichissement-des-donnees-COVID-19-Sante-Publique-France](https://github.com/fcafca/Enrichissement-des-donnees-COVID-19-Sante-Publique-France)

J’ai démarré la réalisation d’une **série de tableaux de bord**, avec l’outil libre et open source Apache Superset qui représente une alternative crédible au « poids lourd » du secteur : Tableau.
[https://github.com/apache/incubator-superset](https://github.com/apache/incubator-superset)
Malheureusement, pour l’instant, je ne dispose pas d’une instance dimensionnée pour proposer un accès public à Superset.
Dans l’attente, je publie ces copies d’écran. Trois thèmes sont abordés, dont l'évaluation du déconfinement :

**Thème 1 : Evaluation du déconfinement depuis le 1er juin (nouvelle version) **

Pour résumer la situation en ce début du mois de Juillet, mis à part en Guyane et à Mayotte, l’épidémie est annoncée globalement maîtrisée.
En revanche, le virus est toujours là. La situation est mesurée par Santé Publique France au travers d’un point hebdomadaire publié en fin de semaine.
Le point central d’attention tourne autour des fameux « clusters », et notre capacité à les traiter au fur et à mesure de leurs apparitions.
Le PDF de l’analyse nationale est pour le moins consistant. 31 pages de graphiques accompagnés de commentaires, pour certains assez « obscurs ».

Exemple, le fameux indicateur "R" qui mesure la diffusion potentielle du virus. On nous rebat les oreilles qu'il doit absolument être inférieur à 1.

"Aucune région métropolitaine ne présente un R significativement supérieur à 1.
Les régions Auvergne-Rhône-Alpes (1,10; IC95% : 0,97-1,25), Bretagne (1,22; IC95% : 0,82-1,69), Normandie (1,01; IC95% : 0,84-1,20) et La Réunion (1,23; IC95% : 0,68-1,95) ont des estimations légèrement supérieures à 1 mais non significativement supérieures (valeur « 1 » comprise dans l’intervalle de confiance)"

De plus, Certaines données ne sont pas publiques, notamment celles qui concernent le détail et la localisation des clusters.
Néanmoins, pour celles qui sont accessibles et issues des trois sources disponibles citées en début de page, je vais tenter de reprendre certains de leurs graphiques, en plus « détaillé ».

Ce dashboard, pour l’instant circonscrit à la région Île-de-France, est un premier jet, une sorte de brouillon que je compte bien améliorer dans les jours à venir.

**09/07 : J’ai ajouté un dashboard spécifique au département de la Mayenne, ou six clusters actifs sont comptabilisés. La semaine prochaine, l’ARS locale a décidé de tester une partie de la population, soit 300 000 habitants.
Les courbes seront à surveiller. Notamment celles relatives aux passages / hospitalisations qui affichent une augmentation, mais avec des chiffres qui restent globalement assez bas.**

"*C'est dans l'angoisse que l'homme prend conscience de sa liberté.*" (Jean-Paul Sartre)
