# Le Coût de la Vie en Colombie : Un Arbitrage Multiple

Ce projet explore le modèle monocentrique comme outil pour comprendre le coût de la vie en Colombie, mettant en évidence à la fois le gradient distance-logement des dépenses et en prenant en compte le facteur de développement.

## Introduction : Motivation et Revue de la Littérature

L'étude du coût de la vie dans les territoires est pertinente dans un contexte où des mouvements sociaux tels que les gilets Jaunes, Insulate Britain et la Covid-19 ont accentué les inégalités socio-spatiales Rodriguez-Pose, 2020). Cette question devient cruciale, surtout dans les pays en développement où les problématiques urbaines nécessitent une attention particulière (Bryan et al., 2020).

### Notre Analyse

Nous utilisons un modèle monocentrique simplifié pour mesurer les effets d'agglomération dans le contexte du développement.

#### Pourquoi le Modèle Monocentrique ?

(a) Ce modèle capture une grande partie de la variabilité du coût de la vie entre territoires, principalement grâce aux postes de consommation logement-transport.
(b) Les effets d'agglomération justifient l'utilisation de ce modèle : l'activité économique, la densité, et les besoins en aménités influencent directement le coût de la vie.

#### Contexte de la Colombie

La Colombie, en tant que pays en développement, présente une grande diversité socio-spatiale avec une possible organisation polycentrique (Tsivanidis, 2023). Cela pose des défis pour le modèle monocentrique et soulève des questions sur sa pertinence. Il s'avère qu'il sera important d'inclure ce facteur de développement afin d'éviter un biais de sur-estimation.

## Plan du Projet

### Collecte et Traitement des Données

Nous utilisons des données ouvertes, l'enquête des ménages en Colombie de 2021 (DANE, 2023). Nous effectuons des opérations de merge sur différentes couches géographiques (capitale, périurbain, rural) pour une analyse spatiale fine. Une attention particulière est portée à la création d'une variable territoriale en fonction de la densité de population.

### Statistiques et Modélisation

Nous réalisons des statistiques descriptives et utilisons des modèles de régression pour explorer les relations entre le coût de la vie, les caractéristiques individuelles et les effets d'agglomération liés au territoire. Nous effectuons d'abord une analyse inter-territoriale pour déterminer la structure de l'urbain en Colombie. D'abord, une analyse inter-territoriale avec une régression linéaire (3_reg_and_tests). Cette regression initiale sera enrichie avec une selection de variable fait par nested LASSO (4_lasso_further_reg) et présentée dans 4_reg_finale. On complémente l'étude inter-territoriale avec un zoom intra-territorial, où nous utilisons une regression pondérée par les poids de sondage (4_reg_intra_territoire)

### Visualisation et Conclusion

La visualisation par cartes des différentes catégories de territoires permet de voir les écarts de dépense en logement à l'intérieur des départements (entre les couches territoriales) et entre les départements. Nous utiliserons aussi les poids de sondage afin de présenter des cartes représentatives du champ étudié. Enfin, nous tirons des conclusions sur la structure urbaine colombienne.

Champ : Population active en Colombie, décembre 2021
Source : DANE (2023)

## Bibliographie



Ce projet s'appuie sur des méthodologies antérieures, en particulier France Strategie (2023), ainsi que sur d'autres travaux connexes.

---

**Note:** Les données brutes sont accessibles via 1_extract_merge_append.
