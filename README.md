***Nouvelle version !!! (09/07) : Ajout d'analyses relatives au déconfinement depuis le 1er Juin*** 

Données actualisées le **29/07/2020**  pour les quatre jeux de données *(sauf pour données relatives aux tests de dépistage)*

**site de téléchargement et d'information** : [https://www.fcafcadata.net/](https://www.fcafcadata.net/)

La réutilisation concerne quatre jeux de données publiés par Santé Publique France: 

**Données hospitalières relatives à l'épidémie de COVID-19**
**Données des urgences hospitalières et de SOS médecins relatives à l'épidémie de COVID-19**
**Données relatives aux tests de dépistage de COVID-19 réalisés en laboratoire de ville** *(production interrompue par SPF depuis le 29/05)*
**Données relatives aux résultats des tests virologiques COVID-19 (SI-DEP)** *(production récente)*

Les quatre jeux de données étant à la granularité du département. **Le référentiel d'enrichissement est donc identique** pour chacun d’entre eux.
Il comporte 17 colonnes qui précèdent celles des données :
Préfecture du dpt, indication de la préfecture de région, latitude et longitude (pour carto), superficie, décès, population INSEE, par tranches d'âge, etc..

J'ai créé un dépôt git : [https://github.com/fcafca/Enrichissement-des-donnees-COVID-19-Sante-Publique-France](https://github.com/fcafca/Enrichissement-des-donnees-COVID-19-Sante-Publique-France)

J’ai démarré la réalisation d’une série de tableaux de bord, avec l’outil libre et open source Apache Superset qui représente une alternative crédible au « poids lourd » du secteur : Tableau.
[https://github.com/apache/incubator-superset](https://github.com/apache/incubator-superset)
Malheureusement, pour l’instant, je ne dispose pas d’une instance dimensionnée pour proposer un accès public à Superset.
Dans l’attente, je publie ces copies d’écran. Trois thèmes sont abordés, dont l'évaluation du déconfinement :

**Thème 1 : Evaluation du déconfinement depuis le 1er juin (nouvelle version)**

Pour résumer la situation en ce début du mois de Juillet, mis à part en Guyane et à Mayotte, l’épidémie est annoncée comme globalement maîtrisée.
En revanche, le virus est toujours là. La situation est mesurée par Santé Publique France au travers d’un point hebdomadaire publié en fin de semaine.
Le point central d’attention tourne autour des fameux « clusters », et notre capacité à les traiter au fur et à mesure de leurs apparitions.
Le PDF de l’analyse nationale est pour le moins consistant. 31 pages de graphiques accompagnés de commentaires, pour certains assez « obscurs ».

https://www.santepubliquefrance.fr/maladies-et-traumatismes/maladies-et-infections-respiratoires/infection-a-coronavirus/documents/bulletin-national/covid-19-point-epidemiologique-du-23-juillet-2020

Certaines données ne sont pas publiques, notamment celles qui concernent le détail et la localisation des clusters.
Pour celles qui sont accessibles et issues des trois sources disponibles citées en début de page, j’ai pour objectif de reprendre certains de leurs graphiques, en plus « détaillé ».

Le dashboard réalisé est un premier jet, une sorte de brouillon que je compte bien améliorer dans les jours à venir.

"*C'est dans l'angoisse que l'homme prend conscience de sa liberté.*" (Jean-Paul Sartre)
