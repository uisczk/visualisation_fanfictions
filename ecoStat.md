# Environnement statistiques - projet données comme écosystème >> modélisation 

>Note : afin de permettre de meilleures appréhension et compréhension des données et du présent projet, nous renvoyons le lecteur à **[une synthèse des recherches](README.md) effectuées pour le M1** qui les met en contexte. Le lecteur trouvera également des éléments de vocabulaire propre aux fanfictions.

## SOURCES DE DONNÉES (DATA BRUTES)
Données collectées dans le cadre du M1 : paradonnées des documents du corpus, et paradonnées de 4 échantillons témoins, accessibles à partir de la page **[AO3StatistiquesMemoire_DataBrutes_AccesPublic](https://docs.google.com/spreadsheets/d/e/2PACX-1vREmUfEGdbl9OCKm1iCf4wxcxwLf8Wagq7iYsRuPtcVX7AApNE42sZ0qr__2sN_8hEG_sLXaNu2MG3M/pubhtml)**.

<ins>Extrait</ins> du tableau de données page tag:MUSEUMS :
| title | author	| posted | language | words | hits | kudos | category | warning | rating | fandom	|
| ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- |
| Brûlons Florence.	| Smokedandelions |	22/11/2021	| Français	| 4301	| 279	| 13 |	M/M | Choose Not To Use Archive Warnings	| Teen And Up Audiences	| Hannibal (TV) |								
| Dangerous Criminal Love	| KiriAsakura	| 30/12/2020	| Español	| 59662	| 1050	| 38	| M/M	| Graphic Depictions Of Violence, Rape/Non-Con	| Explicit	| Hannibal (TV) |
| Legame	| donutgladiator	| 25/03/2021	| Italiano	| 793	| 68	| 3	| M/M	| No Archive Warnings Apply	| General Audiences	| Hannibal (TV)	|												
| living statue	| shycap	| 04/02/2022	| English	| 1672	| 723	| 104	| M/M	| No Archive Warnings Apply	| General Audiences	| Hannibal (TV)	|
| Lord director	| Joseph_Amadeus	| 07/08/2021	| English	| 4090	| 3323	| 303	| M/M	| No Archive Warnings | Apply	Teen And Up Audiences	| Hannibal (TV)	|
| Museums Incite Riots	| blueboxesinmaryland (demoncard)	| 16/09/2014	| English	| 1104	| 3062	| 181	| M/M	| No Archive Warnings Apply	| Not Rated	| Hannibal (TV) |

## DATA TABLES
Renvoyer au fichier (*[ibid.](https://docs.google.com/spreadsheets/d/e/2PACX-1vREmUfEGdbl9OCKm1iCf4wxcxwLf8Wagq7iYsRuPtcVX7AApNE42sZ0qr__2sN_8hEG_sLXaNu2MG3M/pubhtml)*).
>Suite à des difficultés techniques (hardware), l'exploitation de ces données avec Javascript et Jquery est reportée.

## STRUCTURES VISUELLES
Visualisation données sur interface web, pour permettre une accessibilité des données, dans le cadre de la recherche et d'un archivage des pratiques faniques au service des fans. Les données exploitées dans le cadre de ces recherches se divisent en deux types : paradonnées, c'est-à-dire l'ensemble des data autour des textes eux-mêmes (nombre de hits, auteur, classification, etc), et matière textuelle, soit le texte lui-même.
>Pour davantage de détails, se référer à [la synthèse](README.md).

Structures visuelles favorisées pour les paradonnées : 

  - modèles d'après HAYLES et MORETTI.
>MORETTI Franco, *Graphes, cartes et arbres. Modèles abstraits pour une autre histoire de la littérature,* Paris, Les Prairies ordinaires, 2008, [2005].

  - modèles classiques (pie chart, scatterplot, bars) présentés *[ibid.](https://docs.google.com/spreadsheets/d/e/2PACX-1vREmUfEGdbl9OCKm1iCf4wxcxwLf8Wagq7iYsRuPtcVX7AApNE42sZ0qr__2sN_8hEG_sLXaNu2MG3M/pubhtml)*.

  - modèles d'après Mike Bostock, [D3 gallery, Observable](https://observablehq.com/@d3/gallery) :
    - collapsible tree ;
    - connected scatterplot ;
    - parallel sets ;
    - force directed diagram ;
    - revenue by music format diagram ; etc.

Structures visuelles favorisées pour le texte brut : passer par [Voyant Tools](voyant-tools.org).

## REPRÉSENTATIONS DE DONNÉES

Représentation des paradonnées :
  - rapport kudos/hits (*[ibid.](https://docs.google.com/spreadsheets/d/e/2PACX-1vREmUfEGdbl9OCKm1iCf4wxcxwLf8Wagq7iYsRuPtcVX7AApNE42sZ0qr__2sN_8hEG_sLXaNu2MG3M/pubhtml)*) ;
  - partition entre catégories (*[ibid.](https://docs.google.com/spreadsheets/d/e/2PACX-1vREmUfEGdbl9OCKm1iCf4wxcxwLf8Wagq7iYsRuPtcVX7AApNE42sZ0qr__2sN_8hEG_sLXaNu2MG3M/pubhtml)*) ;
  - comparaison des moyennes et médianes des hits, kudos et mots entre le corpus restreint et les corpus témoins ;
  - rapport auteur/reste des paradonnées : favorisation de certaines classifications, catégories, autres ;
  - répartition des langues selon les corpus ; etc.

Représentation de la matière textuelle :
  - rapport tags/occurences dans les textes ;
  - visualisation des dynamiques dans l'économie du texte, comparées entre les langues d'écriture :
    - concentration d'occurences ;
    - champs lexicaux ;
    - candences ; etc.
  

## REPRÉSENTATIONS POUR RÉPONDRE À QUELLES QUESTIONS
  
  - quels sont les profils de documents émergeants, d’après les paradonnées ?
  - quels sont les profils de documents émergeants, d’après la modélisation des textes ?
  - quels rapports à la langue ou aux langues observe-t-on ?
  - quel rapport aux œuvres d'art observe-t-on (voir [synthèse](README.md)) ? Comment s'intègrent-elles dans l'économie des textes, quelles sont leurs conditions d'apparition ?
  

## INTERACTIONS AVEC L'ENVIRONNEMENT

- mise en rapport avec corpus élargi ;
- schématisation multiscalaire ;
- paradonnées ;
- interactions temps long et global ;
- interactions intracorpus ;
- matière textuelle / documents ;
- visualisation entre économie du texte et paradonnées ;
- inscription des fanfictions dans un contexte spécifique de production : notion de *grassroots* (JENKINS), importance des sites d'archives et de partage des textes, *mainstreamisation* des pratiques d'écriture et de partage des fanfictions, etc.

