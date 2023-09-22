---
title: Gérer ses images d’archives avec Tropy
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

Par ailleurs, en plus des collections numérisées par les institutions patrimoniales, les centres d'archives ont progressivement adopté des politiques permissives quant à la possibilité de reproduction photographique de leurs ressources de la part du public. L'époque où il fallait prévoir un petit budget pour effectuer un nombre - parfois limité - de photocopies en papier semble définitivement révolu devant la démocratisation et la généralisation de l'usage d'appareils de reproduction photographique (appareil photo numérique, smartphone, applications de numérisation) y compris à des fins de recherche. Cela ajoute, en réalité, une couche supplémentaire de médiation entre l'historien(ne) et ses sources [^2] soit un défi supplémentaire à apprivoiser. 

La numérisation de la pratique de la collecte des sources historiques, tout comme la transformation de la nature de leur support, ont débouché sur de nouveaux défis concernant l'organisation, l'exploitation et la préservation de ce qui se présente désormais, en grande partie, sous forme de fichiers numériques. Déjà dans sa forme analogique, l'archive se prêtait à la métaphore du flux&#x202F;: &laquo;&#x202F;démesurée&#x202F;&raquo;, &laquo;&#x202F;envahissante comme les marées d'équinoxes, les avalanches ou les inondations&#x202F;&raquo;[^1]. À son tour, l'archive numérique semble presque côtoyer le chaos: 

> &laquo;&#x202F;[...] L'impératif de photographier le plus possible [de documents] amène à dissocier les objets de leur contexte, atomise les documents en les transformant en fragments et, tout en promettant l'abondance, débouche sur du chaos [...]. Il n'existe pas de solution technologique rapide [...] pour les chercheurs et chercheuses à la dérive devant une mer silencieuse de fichiers JPG&#x202F;&raquo;[^3]. 

Tropy vise donc à offrir une infrastructure legère à la portée des historiennes et des historiens pour répondre aux besoins concrets qui émergent lors des phases de collecte et d'analyse des sources historiques qui se présentent sous forme de fichiers d'images en provenance de divers centres d'archives et souvent de formats hétéroclites (PDF, formats images tels JPEG, PNG etc). En particulier, il s'agit d'offrir une interface spécifique pour (re)construire l'archive d'une recherche spécifique afin d'effectuer les opérations suivantes&#x202F;: 
* rassembler des photos de documents ou d'autres sources primaires faits à l'issue de séjours aux centres d'archives ou obtenues à partir de collections numériques disponibles en ligne ou encore collectées de ses propres moyens     
* classifier et organiser ces matériaux en séries qui ont du sens pour une recherche spécifique 
* contextualiser ses sources en attribuant aux fichiers images qui les représentent des métadonnées d'origine (par exemple date d'un document, série et sous-série du fonds d'archive dont il provient...)    
* annoter ses sources sachant que la possibilité est offerte de fournir des transcriptions, de prendre des notes, et d'indexer à la fois les photos et les données qui émanent de ces opérations supplémentaires. 

## Présentation du corpus d'images d'archives: les affiches de Mai 68
Nous allons découvrir coment travailler avec Tropy en utilisant un corpus d'images numérisées et disponibles en ligne sur le site de [Gallica](http://gallica.bnf.fr/), la bibliothèque numérique de la Bibliothèque nationale de France et (ci-après BnF) et de ses institutions partenaires. Notre corpus se compose d'environ quatre cents affiches numérisées de [Mai 1968 en France](https://fr.wikipedia.org/wiki/Mai_68). Ces affiches, à l'origine des [sérigraphies](https://fr.wikipedia.org/wiki/S%C3%A9rigraphie) pour la plupart, ont été principalement des créations du dit [Atelier populaire de l'Ecole des Beaux-Arts](https://www.persee.fr/doc/mat_0769-3206_1988_num_11_1_403852) à Paris lors de l'occupation de cette école en mai-juin 1968, mais aussi d'ateliers du même type qui se sont constitués dans d'autres villes (Montpellier, Marseille...). Plusieurs bibliothèques et musées disposent des bribes des affiches de mai 68 dans leurs collections, toutefois Gallica donne accès à une collection numérisée quasi-complète qui rassemble des items physiquement présents dans diverses institutions. Ces numérisations datent des années 2010 et font partie des opérations en masse qui ont constitué le patrimoine numérique français à l'époque qui a suivi l'inauguration du projet de Google Library (aujourd'hui abandonné). Elles témoignent aussi de la patrimonialisation de l'évènement de mai 68 et de l'effet de celle-ci sur la création et mise à disposition de la source numérisée. Les fichiers images des affiches sont téléchargeables en format PDF ou JPEG depuis le site de Gallica.        

 
## Démarrer avec Tropy 

### Installer Tropy 
Tropy peut être librement téléchargé depuis son [site web](https://tropy.org/). C'est un logiciel multi-plateformes (Linux, Windows, macOS) et son installation se fait en local&#x202F;; pour le moment il n'est pas possible de l'installer sur un serveur partagé et travailler à plusieurs. Notre leçon mobilise la version 1.14.0 de Tropy. 

### Préparer son corpus d'images d'archives
Vous pouvez suivre cette leçon soit en utilisant le corpus des images d'affiches de Mai 1968 ou en privilégiant un corpus de votre préférence y compris vos propres images d'archives. Dans le premier cas, merci de suivre les instructions que nous fournissons sur comment obtenir ces fichiers. *(N.D.L.A. Ces instructions seront ajoutées une fois que le brouillon de la leçon aura intégré le jeu de données)*

Si vous préférez utiliser vos propres sources, n'hésitez pas à commencer avec le fruit d'une journée de travail au centre d'archives de votre préférence&#x202F;: des centaines de fichiers de photos en forme brute, que vous venez de copier depuis votre smartphone sur votre disque dur, sans même avoir eu le temps de les renommer, et qui attendent patiemment votre attention. C'est le moment de s'en occuper&#x202F;!    

## Créer et configurer un projet

### Se répérer entre les éléments de base d'organisation d'un projet dans Tropy 
Avant de commencer, il est important de comprendre les éléments de base de la structure d'un projet dans Tropy. Ces éléments sont les suivants&#x202F;: 
* projet
* objet 
* liste
* tag (soit libellé)

Le projet est votre projet de recherche, de publication, de crowdsourcing... tout projet intellectuel autour d'un sujet qui englobe un ensemble de sources que vous souhaitez exploiter dans ce cadre et dont vous disposez sous forme de fichiers images. C'est aussi votre point d'entrée dans l'interface de Tropy pour accéder aux photos d'archives qui lui correspondent afin de les organiser et d'effectuer nombre d'opérations en vue de leur analyse. 

L'objet dans Tropy est essentiellement votre source&#x202F;: un document d'archives, un monument, une œuvre d'art, une affiche... Un objet équivaut à une ou plusieurs photos: par exemple, dans le cas d'un document d'archives de plusieurs pages, vous avez peut-être des photos séparées de chaque page. Lorsque vous créez l'objet qui correspond à ce document dans Tropy, celui-ci englobera les photos de toutes les pages et comptera comme une unité.   

Les objets peuvent s'organiser en listes&#x202F;; par liste, dans Tropy, il faut entendre une série, ou une sous-partie si vous préférez, que vous constituez en rassemblant plusieurs objets qui partagent une caractéristique commune selon la problématique de votre projet. Par exemple, si vous travaillez sur la création artistique d'une certaine période, vous pouvez constituer des listes selon les avant-gardes de la période en question ou selon artiste ou encore en appliquant des critères géographiques.   

Enfin, dernier élément de base d'importance, le libellé, que vous trouverez dans l'interface comme &laquo;&#x202F;tag&#x202F;&raquo;. Nous le verrons plus en détail par la suite, les tags sont des moyens d'indexation personnelle](https://fr.wikipedia.org/wiki/Folksonomie) des objets que nous créons dans Tropy. Cette indexation peut être thématique ou fonctionnelle, à vous d'inventer le système qui vous convient. Bien indexer nos sources au moment de les enregistrer peut parfois être jugé chronophage. En réalité, c'est du temps gagné que nous récupérons lors de l'analyse et de la rédaction en facilitant l'accès, de manière transversale, à des sources qui font partie de différentes listes mais qui sont réunies par une caractéristique commune.     

### Créer un projet
Lançons Tropy - comme vous le verrez, nous avons aussitôt accès à une boîte de dialogue et, en haut, au menu principal. La boîte nous invite à créer un projet, d'abord en le nommant puis en sélectionnant son type&#x202F;: standard ou avancé - nous allons voir de quoi il s'agit [dans un moment](#configurer-un-projet). Nous pouvons aussi créer notre projet à partir du menu principal&#x202F;: Fichier > Nouveau > Projet. Nous n'allons pas explorer davantage le menu à ce point, sauf si nous souhaitons [paramétrer la langue de l'interface](#paramétrer-la-langue). 

Créons donc notre projet en lui attribuant le titre de notre préférence -  le nôtre s'appelle Affiches de Mai-Juin 1968. 

### Configurer un projet: choisir entre standard et avancé
Tout en le créant, il faut définir si nous souhaitons que notre projet soit de type standard ou avancé - l'option par défaut étant standard. De quoi s'agit-il exactement&#x202F;? Le type de projet est [une fonctionnalité disponible à partir de la version 1.14.0 de Tropy](https://tropy.org/blog/new-project-types-in-tropy-1-13). 

Un projet standard, au moment de l'importation des fichiers des images, crée aussitôt des copies des ces images pour les stocker dans un répertoire spécifique de Tropy. L'avantage dans ce cas est que notre projet devient intégralement portable - par exemple, en le copiant sur une clé USB et en l'important dans un autre environnement de travail, nous pouvons le retrouver tel que nous l'avions laissé dans son environnement d'origine, et continuer à travailler dessus sans interruption. L'inconvénient d'un projet standard est qu'il nécessite des machines performantes et beaucoup de mémoire disponible, car les fichiers images sont des fichiers lourds. 

De son côté, un projet avancé n'effectue pas de copies des images d'origine, celles-ci ne sont donc pas stockées dans un répertoire intégré au projet, même si nous pouvons toujours les voir via l'interface de Tropy. Ici, comme il le faisait dans ses versions précédentes, Tropy établit des liens, ou plutôt des chemins, vers les répertoires d'origine dans lesquels nous conservons nos fichiers à l'emplacement de notre choix. Ainsi, les projets avancés sont des projets plus légers, puisqu'ils ne contiennent que les données que nous ajoutons (structure, notes, libellés, transcriptions...). En revanche, pour assurer la portabilité d'un projet avancé, il faudra veiller à l'accompagner, dans son nouvel environnement, des répertoires séparés de nos images et d'intervenir pour rétablir les chemins cassés, le cas échéant. Si vous ne souhaitez pas mettre la main dessus ou ne savez pas trop comment s'y prendre, il vaut mieux sélectionner le mode standard.    

À vous de choisir quelle est l'option qui vous convient le plus, sachant que pour suivre les étapes suivantes de cette leçon, le choix de type de projet n'a pas vraiment d'incidence. En ce qui nous concerne, nous optons pour créer un projet avancé pour éviter d'avoir un projet lourd, mais, encore une fois, le choix vous appartient selon vos propres contraintes et préférences.

Admettons que nous avons créé notre projet, par défaut celui-ci est stocké dans le répertoire `Documents` et son extension est .TPY. Il est tout à fait possible de sauvegarder un projet Tropy à l'emplacement de notre préférence que nous choisirons via la boîte de dialogue qui s'ouvre après avoir entré le nom de notre projet et appuyé sur le bouton Create Project. Par ailleurs, c'est peut-être aussi le moment de profiter de [la leçon sur les bonnes pratiques d'organisation des fichiers des données d'une recherche](/fr/lecons/preserver-ses-donnees-de-recherche)&#x202F;!            

### Paramétrer la langue 
Tropy est disponible dans plusieurs langues dont le français. Pour paramétrer la langue à laquelle nous souhaitons que l'interface soit disponible, rendons-nous, à partir du menu principal, à Édition > Préférences > Paramètres. Une fois là, il est possible de sélectionner la langue de notre préférence à partir de la liste déroulante. 

## Importer ses sources
Nous partons du principe que vous avez déjà des photos de vos archives ou que vous avez récupéré celles que nous fournissons avec la leçon. 

### Parcourir l'interface du projet 
Une fois notre projet créé et lancé, nous nous trouvons face à l'interface à partir de laquelle nous allons effectuer les principales opérations le concernant&#x202F;: l'interface du projet. L'autre interface principale via laquelle nous travaillerons est celle de l'objet, mais nous n'en sommes pas encore là&#x202F;! De l'interface du projet nous avons accès au menu principal en haut; à un menu latéral à gauche d'où nous accédons toujours à l'interface au projet, aux listes créées, mais aussi aux dernières importations que nous effectuons au fur et à mesure, aux tags et aux objets supprimés. Depuis la zone du milieu, nous avons une vue d'ensemble des objets de notre projet et nous pouvons accéder à chacun d'eux pour les inspecter mieux et ce de deux façons. En plaçant le curseur de notre souris sur un objet, nous faisons afficher, dans le menu latéral à droite, des informations qui lui sont spécifiques: métadonnées, tags, le(s) fichier(s) de photo(s) qui se rapportent à cet objet.

### Importer les fichiers des images 
Il est possible d'importer les fichiers des images de deux façons. Soit les glisser, un par un ou en les sélectionnant tous, directement dans la zone du milieu du menu, réservée aux objets; soit utiliser le menu principal. Pour le faire depuis le menu, aller à Fichier > Importer > Photos, pour importer un ou plusieurs fichiers d’images depuis un répertoire; ou à Fichier > Importer > Dossier, si vous souhaitez importer tout un répertoire de fichiers. 

Les formats de fichiers que Tropy peut prendre en charge les principaux formats qui peuvent abriter des images dont JPG/JPEG, PNG, SVG, TIFF, GIF, PDF (pour une liste complète se référer à la documentation du projet). 

### Importer des images depuis une page web
Il est possible d'importer des images statiques qui ont leur propre URL directement depuis une page web dans un projet Tropy. Pour ce faire, il faut se positionner dans l'interface du projet et glisser l'image sélectionnée depuis le navigateur vers la zone du milieu de l'interface offrant une vue d'ensemble des objets. Attention, l'importation est différente selon que le type du projet soit standard ou avancé. Si le projet est standard, Tropy effectue aussi une copie de l'image qui est ainsi téléchargée au cours de l'opération et intégrée dans le projet. En revanche, si le projet est en mode avancé, seulement un lien est créé vers l'adresse web de l'image, sans que celle-ci ne soit téléchargée. Dans ce cas, il faut soit double-cliquer sur l'objet créé dans notre interface pour accéder, via le web, à l'image d'origine soit effectivement la télécharger de son emplacement d'origine et la copier dans un répertoire sur notre disque dur pour ensuite l'importer dans le projet. 

Enfin, il faut noter que les opérations décrites ci-dessous sont possibles seulement avec les formats d'images statiques mais pas avec les fichiers PDF. Il faudra télécharger ces derniers pour ensuite pouvoir les intégrer dans iun projet Tropy. De même, lorsque les images sont accessibles via des pages dynamiques, comme le sont les pages générées via un moteur de recherche, il n'est pas possible de les importer directement dans Tropy. C'est en grande partie le cas d'images auxquelles nous accédons à la suite de recherches dans des bibliothèques numériques, et c'est aussi celui de notre corpus, que nous avons pris soin de télécharger afin de pouvoir l'utiliser. Comme bonne pratique, nous conseillons de télécharger et de sauvegarder en local les corpus qui constituent vos données de recherche.        
<!--
### Orientation
-->


## Décrire ses sources
Au moment d'importer les images, il est judicieux de les décrire avec les métadonnées d'origine des sources primaires qu'elles représentent, pour être ensuite en mesure de les exploiter (identifier les documents et y accéder, les analyser, pouvoir les citer...). 

### Métadonnées: kézako? 
Avant toute chose, faisons, très brièvement, le point sur les métadonnées&#x202F;! Les métadonnées sont des informations qui décrivent d'autres données et qui deviennent signifiantes dans un système défini. Dans un cadre scientifique, comme le nôtre, [les métadonnées servent à décrire les données de recherche et les productions réalisées après leur analyse (par ex. articles, livres etc.)](https://doranum.fr/metadonnees-standards-formats/metadonnees-standards-formats-fiche-synthetique_10_13143_vbjs-6288/). Les métadonnées de base auxquelles nous avons affaire dans le cadre de notre projet peuvent porter sur le titre, le créateur ou la créatrice de la ressource qui nous intéresse (une oeuvre d'art, un document diplomatique), la date de création, parfois des destinataires ou encore davantage, comme nous le verrons par la suite.      

### Attribuer des métadonnées par lot
Il est possible d'attribuer des métadonnées aux objets soit à l'unité soit par lot, si nos objets sont homogènes (par exemple, s'il s'agit d'un ensemble de photos de documents en provenance de la même archive, série et sous-série, carton...). C'est le cas de notre corpus, nous pouvons donc attribuer les principales métadonées, en tout cas celles qui sont communes, par lot. Pour ensuite attribuer, au niveau d'objet si besoin, des métadonnées spécifiques si elles ne sont pas communes pour l'ensemble. 

Une bonne pratique pour attribuer des métadonnées communes à un lot de photos est de se positionner au niveau de la dernière importation (accessible depuis le menu à gauche via l'interface du projet). Dans notre cas, la dernière importation est aussi notre importation originelle, mais il s'agit d'une bonne pratique à adopter. Au fil d'un projet, plusieurs importations de fichiers d'images peuvent se faire de manière différée, selon la temporalité d'une recherche, successivement à la suite d'une série de séjours dans différents centres d'archives... Cela veut dire qu'un projet peut s'étendre au fil du temps pour englober plusieurs importations de fichiers. Si des métadonnées sont attribuées à la suite de chaque importation, il n'est pas nécessaire de revenir sur ces anciennes couches à nouveau, au contraire il vaut mieux les préserver. C'est ce que nous faisons en nous positionnant au niveau de la dernière importation. 

*(Description comment attribuer de manière groupée des métadonnées avec aussi un exemple d'attribution de métadonnées plus spécifiques au niveau de l'objet en se rapportant à notre corpus d'affiches).* 
Depuis l'interface du projet, nous nous plaçons au niveau de la zone du milieu avec la vue d'ensemble des objets que nous avons importés. Nous les sélectionnons tous, que ce soit depuis l'affichage en mode liste ou vignette, Ensuite, nous accédons au menu qui se trouve dans la partie droite de notre écran pour aller à ce qui se présente comme une fiche Métadonnées. Pour le moment, cette boîte de dialogue est de type Tropy Generic, si nous nous fions à son intitulé - cela peut changer depuis la liste déroulante, mais restons là pour l'instant. Cette boîte comporte une liste de champs cliquables que nous pouvons peupler d'informations. Nous identifions comme informations communes à tous les objets de notre corpus les champs source, collection, droits. Nous allons donc renseigner chacun de ces champs. Les métadonnées sont appliquées à tous les objets sélectionnés. 

### Attribuer des métadonnées par objet
       


### Sélectionner, personnaliser le modèle de saisie des métadonnées
### Champs non-modifiables
### Vocabulaires contrôlés

## *Visualizing/Viewing and Annotating Items*
### *Editing for Legibility*
### *Selections*
### *Notes*

## Organizing your Tropy Project
_We could remind here to the readers that main elements one meets in Tropy are: Project, Object, List, Tag. I think it is important to underline that one object = one document (and that several pages, and so ohotos of the pages, can compose one object_. 
### Lists
### Tags

## Custom Workflows and Extensions for your Tropy Project
### Core plugins
#### IIIF
#### Omeka
#### CSL
#### CSV
#### Archive





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

[2^] Frédéric Clavert, &laquo;&#x202F;Introduction&#x202F;&raquo; in Frédéric Clavert & Caroline Muller (dir.), *Le goût de l’archive numérique*,
https://gout-numerique.net/

[^3] Sean Takats, &laquo;&#x202F;Tropy&#x202F;&raquo;, billet de blog, _Quintessence of Ham_, 26 octobre 2017, http://quintessenceofham.org/2017/10/26/tropy date de consultation 1<sup>er</sup> septembre 2023

