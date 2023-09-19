---
title: Gérer ses photos d’archives avec Tropy
collection: lessons
layout: lesson
slug: tropy-fr
date: 2023-09-01
authors:
- Sofia Papastamkou
- Anita Lucchesi
- Douglas McRae
reviewers:
- 
editors:
- 
translator:
review-ticket: 
difficulty: 1
activity: analyze
topics: [data-manipulation, data-management]
abstract: "Apprendre à organiser, annoter et préparer l'utilisation à des fins de recherche des photos de vos sources primaires à l'aide de Tropy."
avatar_alt: 
doi: 
---

{% include toc.html %}

## Présenter Tropy en un clin d'oeil

<!--what-->
[Tropy](https://tropy.org/) est un logiciel de gestion d'images numériques de matériaux de recherche&#x202F;: à comprendre des photos de documents d'archives, de monuments, d'oeuvres d'art et, au final, de tout type de source primaire représentée sous forme d'image numérique, selon bien évidemment le contexte de recherche dans lequel elle s'insère. 
<!--who-->
Il s'agit d'un logiciel conçu et développé depuis 2016 au sein d'établissements d'enseignement supérieur et de recherche interdisciplinaires, tel le Centre pour l'histoire et les nouveaux médias [Roy Rosenzweig](https://rrchnm.org/tropy/) de l'université George Mason (Virginie, Etats-Unis), et le Centre pour l'histoire contemporaine et digitale de l'université du Luxembourg. Il bénéficie en outre de l'appui de l'organisation à but non lucratif Digital Scholar (qui soutient également les logiciels Zotero et Omeka). Tropy est un logiciel à code ouvert (accessible sur le dépôt GitHub) dont l'utilisation est gratuite. Il peut être librement téléchargé à partir de son [site web](https://tropy.org/) - ce que nous recommandons de faire à celles et ceux qui souhaitent suivre cette leçon. 
<!--about-->
En ce qui concerne la documentation d'utilisation, un guide  officiel est [disponible en anglais](https://docs.tropy.org/) dont une traduction partielle (officieuse) en français, effectuée en 2019, peut s'avérer utile pour le lectorat francophone. Il existe aussi divers tutoriels dont certains audiovisuels. Si vous souhaitez en savoir plus, merci de consulter la [section afférente des références bibliographiques](#références-bibliographiques--tutoriels-et-ressources-éducatives-en-français) <!-- vérifier le lien ancre-->.
De surcroît, un [forum Tropy](https://forums.tropy.org/) existe aussi pour les utilisatrices et les utilisateurs qui souhaitent aborder des questions spécifiques avec la communauté (notamment en anglais). Par ailleurs, Tropy dispose d'une [chaîne sur YouTube](https://www.youtube.com/channel/UCQ3QCuNGz825BGSHG9JryeA) - à présent il existe des ressources en anglais et en espagnol, mais pas en français. Enfin, Tropy est présent sur les principaux réseaux sociaux en ligne - davantage d'informations sont disponibles sur son site web.     

## Pourquoi utiliser Tropy? 

Tropy a été spécialement conçu par et pour des historiennes et des historiens. Son objectif étant de répondre à l'évolution des pratiques de collecte et d'organisation des sources historiques à l'ère numérique - voire aux mutations des formats de ces sources.  

Effectivement, à partir des années 2000, les bibliothèques et les archives numériques se sont progressivement multipliées. Ainsi, au moins dans certains pays du monde, les infrastructures nécessaires ont été mises en place pour, d'une part, lancer la numérisation des collections patrimoniales et, d'autre part, les mettre à disposition du public à distance. Il serait sans doute illusoire de croire que tout est numérisé, toutefois une partie considérable des collections patrimoniales - et par conséquent des principaux matériaux de recherche en histoire et à portée des chercheur et des chercheuses - l'est. 

Par ailleurs, en plus des collections numérisées par les institutions patrimoniales, les centres d'archives ont progressivement adopté des politiques permissives quant à la possibilité de reproduction photographique de leurs ressources de la part du public. L'époque où il fallait prévoir un petit budget pour effectuer un nombre - parfois limité - de photocopies en papier semble définitivement révolu devant la démocratisation et la généralisation de l'usage d'appareils de reproduction photographique (appareil photo numérique, smartphone, applications de numérisation) y compris à des fins de recherche. 

La numérisation de la pratique de la collecte des sources historiques, tout comme la transformation de la nature de leur support, ont débouché sur de nouveaux défis concernant l'organisation, l'exploitation et la préservation de ce qui se présente désormais, en grande partie, sous forme de fichiers numériques. Déjà dans sa forme analogique, l'archive se prêtait à la métaphore du flux&#x202F;: &laquo;&#x202F;démesurée&#x202F;&raquo;, &laquo;&#x202F;envahissante comme les marées d'équinoxes, les avalanches ou les inondations&#x202F;&raquo;[^1]. À son tour, l'archive numérique semble presque côtoyer le chaos: 

> &laquo;&#x202F;[...] L'impératif de photographier le plus possible [de documents] amène à dissocier les objets de leur contexte, atomise les documents en les transformant en fragments et, tout en promettant l'abondance, débouche sur du chaos [...]. Il n'existe pas de solution technologique rapide [...] pour les chercheurs et chercheuses à la dérive devant une mer silencieuse de fichiers JPG&#x202F;&raquo;[^2]. 

Tropy vise donc à offrir une infrastructure à la portée des historiennes et des historiens pour répondre aux besoins concrets qui émergent lors des phases de collecte et d'analyse des sources historiques qui se présentent sous forme de fichiers d'images en provenance de divers centres d'archives et souvent de formats hétéroclites (PDF, formats images tels JPEG etc). En particulier, il s'agit d'offrir une interface spécifique pour (re)construire l'archive d'une recherche spécifique afin d'effectuer les opérations suivantes&#x202F;: 
* rassembler des photos de documents ou d'autres sources primaires faits à l'issue de séjours aux centres d'archives ou obtenues à partir de collections numériques disponibles en ligne ou encore collectées de ses propres moyens     
* classifier et organiser ces matériaux en séries qui ont du sens pour une recherche spécifique 
* contextualiser ses sources en attribuant aux fichiers images qui les représentent des métadonnées d'origine (par exemple date d'un document, série et sous-série du fonds d'archive dont il provient...)    
* annoter ses sources sachant que la possibilité est offerte de fournir des transcriptions, de prendre des notes, et d'indexer à la fois les photos et les données qui émanent de ces opérations supplémentaires. 

<!-- la partie Installer Tropy n'existe pas dans les autres versions--> 
## Installer Tropy 
Tropy peut être librement téléchargé depuis son [site web](https://tropy.org/). C'est un logiciel multi-plateformes (Linux, Windows, macOS) et son installation se fait en local&#x202F;; pour le moment il n'est pas possible de l'installer sur un serveur partagé. Notre leçon mobilise la version 1.14.0 de Tropy. 







## Références bibliographiques 

Emmanuel Mourlon-Druol, "Déstructuration et restructuration de l’archive à l’ère numérique", billet de blog, site web d'Emmanuel Mourlon-Druol, 7 novembre 2019, URL: https://www.e-mourlon-druol.com/destructuration-et-restructuration-de-larchive-a-lere-numerique/ date de consultation 1er septembre 2023



### Tutoriels et ressources éducatives en français

Cécile Arènes, Meriç Akdogan, & Aurélien Moisan. Tropy , un outil pour gérer les corpus iconographiques. Love Data Week Sorbonne Université. Zenodo. 17 février 2023 https://doi.org/10.5281/zenodo.7656554

Benjamin Laillier, Tutoriel Tropy (version 4), août 2019 http://doi.org/10.5281/zenodo.3381981 

“Tropy | Gestion d’images”, wiki Pole-Num-Scrums-Skills, https://wikis.univ-lille.fr/proj-polnum/accueil/manuels/guide-d-utilisation-de-tropy 

Delphine Valmalle, “Utiliser Tropy pour la gestion de ses photos d'archives”, YouTube, Geneatech, 22 février 2021, https://youtu.be/AiPqbdwP67E  

<!-- en anglais “Tropy Webinar, June 16, 2020 (unedited recording)”, YouTube, Tropy Project, https://youtu.be/jWjP90EWHkQ --> 

## Notes 

[^1] Arlette Farge, *Le goût de l'archive*, Paris, Éditions du Seuil, 1989, 10.  
 
[2^] Sean Takats, "Tropy", billet de blog, _Quintessence of Ham_, 26 octobre 2017, http://quintessenceofham.org/2017/10/26/tropy date de consultation 1<sup>er</sup> septembre 2023