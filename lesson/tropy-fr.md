---
title: Du chaos à l'ordre ou comment gérer des images numériques de sources primaires avec Tropy
collection: lessons
layout: lesson
slug: tropy-fr
date: 2024-08-15
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
abstract: "Apprendre à organiser et annoter des images numériques de sources primaires à l'aide du logiciel Tropy en anticipant leur analyse à des fins de recherche scientifique."
avatar_alt: 
doi: 
---

{% include toc.html %}

## Présenter Tropy en un clin d'oeil
<!--what-->
[Tropy](https://tropy.org/) est un logiciel qui permet de gérer les images numériques de [sources primaires](https://fr.wikipedia.org/wiki/Source_(information)#Source_primaire) tels les documents d'archives, les monuments, les &oelig;uvres d'art ou, au final, tout ce qui, dans un contexte de recherche précis, constitue une source dont on dispose sous forme d'image numérique. Il s'agit d'un logiciel à code source ouvert et gratuit qui peut être librement téléchargé à partir de son [site web](https://tropy.org/) - ce que nous recommandons de faire à celles et ceux qui souhaitent exécuter cette leçon.
<!--who-->
 Le logiciel a été conçu et développé depuis 2016 au sein d'établissements d'enseignement supérieur et de recherche interdisciplinaires, tel le Centre pour l'histoire et les nouveaux médias [Roy Rosenzweig](https://rrchnm.org/tropy/) de l'université George Mason (Virginie, Etats-Unis) et le [Centre pour l'histoire contemporaine et digitale](https://www.uni.lu/c2dh-fr/) de l'université du Luxembourg. Tropy bénéficie en outre de l'appui de l'organisation à but non lucratif [Digital Scholar](https://digitalscholar.org/) qui promeut la production et diffusion de logiciels à code source ouvert à des fins d'usage académique.  
<!--about-->
En ce qui concerne la documentation d'utilisation, un guide officiel est [disponible en anglais](https://docs.tropy.org/). De surcroît, un [forum Tropy](https://forums.tropy.org/) existe aussi pour les utilisatrices et les utilisateurs qui souhaitent aborder des questions spécifiques avec la communauté (notamment en anglais). Par ailleurs, Tropy dispose d'une [chaîne sur YouTube](https://www.youtube.com/channel/UCQ3QCuNGz825BGSHG9JryeA) proposant des vidéos éducatives notamment en anglais et en espagnol, mais pas en français. Enfin, Tropy est présent sur les principaux réseaux sociaux en ligne - davantage d'informations sont disponibles sur son site web.  
Pour le lectorat francophone, [la traduction partielle et officieuse de la documentation du logiciel](http://doi.org/10.5281/zenodo.3381981), effectuée en 2019, peut s'avérer utile. De même, divers tutoriels dont certains audiovisuels sont disponibles en ligne. Pour en savoir plus sur ces ressources produites au sein de la communauté francophone, merci de consulter la [section afférente des références bibliographiques](#tutoriels-et-ressources-éducatives-en-français).   

## Pourquoi utiliser Tropy 
Tropy est une application assez unique en son genre qui permet d'organiser et annoter à partir d'une seule interface les fichiers images de sources primaires. Son avantage est d'avoir été spécialement conçue pour répondre à l'évolution des pratiques de collecte et d'organisation des sources historiques à l'ère numérique afin de faciliter leur organisation et exploitation à des fins d'analyse. 

Pourquoi donc recourir à une application spécifique, alors qu'il est tout à fait possible de s'appuyer sur des systèmes d'organisation de fichiers plus traditionnels et tout aussi efficaces&#x202F;? C'est ce que nous décrivent en tout cas d'expérience un historien de l'intégration européenne [sur son blog](https://www.e-mourlon-druol.com/destructuration-et-restructuration-de-larchive-a-lere-numerique/) ou encore une historienne de la Première guerre mondiale [dans une bande dessinée](https://www.uni.lu/c2dh-fr/news/gazengel-ooooh-tropy/). 

> Si vous pensez être plus adepte d'un système d'organisation classique de vos fichiers sur votre disque dur - sans oublier de sauvegarder régulièrement sur un autre support&#x202F;! - et hésitez de vous lancer pour le moment dans des nouveautés, vous avez intérêt à vous diriger vers [la leçon sur les bonnes pratiques d'organisation des fichiers des données d'une recherche](/fr/lecons/preserver-ses-donnees-de-recherche)&#x202F;! 

L'avènement des technologies web a favorisé l'émergence et la multiplication, surtout depuis les années 2000, des bibliothèques et des archives numériques. Des vagues successives de numérisation de masse, la mise en place d'infrastructures de stockage et de publication électronique y compris des protocoles et standards de description, ont rendu les collections patrimoniales accessibles à distance et, souvent, libres à télécharger. Par conséquent, de plus en plus de "matériaux" utilisés dans la recherche historique sont disponibles sous forme de fichiers numériques dont il est possible d'obtenir des copies et d'utiliser à volonté *a minima* à des fins de recherche personnelle, sinon de partage. Certes, il serait illusoire de croire que tout est numérisé&#x202F;: à titre d'exemple, en France, les fonds numérisés des trois services d'archives à compétence nationale (Archives nationales, départementales et régionales) totalisaient en 2020 environ cinq cents millions de documents textuels et iconographiques dont l'ensemble n'était pourtant pas accessibles en ligne [^4]. Sans connaître vraiment la part précise sur le total des archives conservées, ces documents sont estimés [représenter &laquo;&#x202F;un pourcentage minime&#x202F;&raquo; des collections conservées par ces archives](https://web.archive.org/web/20230306052912/https://www.culture.gouv.fr/Actualites/Histoire-memoire-comment-les-archives-s-ouvrent-au-plus-grand-nombre). Néanmoins, les historiens et les historiennes doivent désormais composer avec une masse de fonds d'archives numérisées qui va croissant.        

En outre, les centres d'archives ont progressivement adopté des politiques plus permissives quant à la possibilité de reproduction photographique de leurs ressources de la part du public. L'époque où il fallait prévoir un petit budget pour effectuer un nombre - parfois limité - de photocopies en papier semble définitivement révolu devant la démocratisation et la généralisation de l'usage d'appareils de reproduction photographique (appareil photo numérique, smartphone, applications de numérisation) y compris à des fins de recherche. Il s'agit, en réalité, d'une couche supplémentaire de médiation entre l'historien(ne) et ses sources [^2], qui se trouvent extraites de leur contexte d'origine puis reconstruites selon la problématique de recherche dont elles font partie. En d'autres mots, l'historien ou l'historienne a la possibilité de constituer sa propre archive hybride à partir des sources numérisées par les institutions patrimoniales ou par ses propres soins, plutôt que de disposer de son corpus de sources en différents formats.     

Par ailleurs, la numérisation à la fois de la source historique et de la pratique de sa collecte, mais aussi la génération de données secondaires (annotations, données d'analyse...), ont débouché sur de nouveaux défis concernant l'organisation, la gestion et la préservation de l'ensemble de ces données de recherche de plus en plus volumineuses. Déjà dans sa forme analogique, l'archive se prêtait à la métaphore du flux&#x202F;: &laquo;&#x202F;démesurée&#x202F;&raquo;, &laquo;&#x202F;envahissante comme les marées d'équinoxes, les avalanches ou les inondations&#x202F;&raquo;[^1]. À son tour, l'archive numérique semble presque côtoyer le chaos&#x202F;: 

> &laquo;&#x202F;[...] L'impératif de photographier le plus [de documents] possible amène à dissocier les objets de leur contexte, atomise les documents en les transformant en fragments et, tout en promettant l'abondance, débouche sur du chaos [...]. Il n'existe pas de solution technologique rapide [...] pour les chercheurs et chercheuses à la dérive devant une mer silencieuse de fichiers JPG&#x202F;&raquo;[^3]. *(N.D.L.R. L'extrait a été librement traduit de l'anglais par les soins de l'auteure de la leçon en français).*

Tropy vise donc à offrir une infrastructure legère à la portée des historiennes et des historiens pour répondre aux besoins concrets qui émergent lors des phases de collecte puis d'organisation et d'analyse des sources historiques sous forme de fichiers d'images numériques. Cette infrastructure logicielle permet d'abriter des fichiers en provenance de divers centres d'archives, et donc de combiner de différentes temporalités d'une recherche, avec aussi l'avantage de faire côtoyer des formats hétéroclites (PDF, formats images tels JPEG, PNG etc). Ainsi, il s'agit d'un dispositif logiciel spécifique permettant de (re)construire l'archive d'une recherche donnée afin d'effectuer les opérations suivantes&#x202F;: 
* rassembler des photos de documents ou d'autres sources primaires faites lors de séjours aux centres d'archives ou obtenues à partir de collections numériques disponibles en ligne ou encore collectées de ses propres moyens   
* classifier et organiser ces matériaux en séries qui ont du sens pour une recherche spécifique 
* contextualiser ses sources en attribuant aux fichiers images qui les représentent des métadonnées d'origine (date d'un document, série et sous-série du fonds d'archive de provenance...)    
* annoter les sources, produire des transcriptions, prendre des notes, indexer à la fois les photos et les données qui émanent de ces opérations supplémentaires
* croiser de manière relativement facile et intuitive des sources lors de la phase de la rédaction d'un travail de recherche, ce qui permet d'optimiser le temps consacré à la rédaction.  

## Le jeu de données
L'ambition de cette leçon était de proposer un jeu de données de sources visuelles pertinentes pour un public francophone. La tâche s'est néanmoins avérée extrêmement compliquée à cause des restrictions appliquées sinon à la collecte, sûrement à la réutilisation et au partage des images en provenance d'archives institutionelles ou de réseaux sociaux numériques. L'auteure de cette leçon a opté pour exposer franchement ces difficultés à des fins pédagogiques concernant l'utilisation ou réutilisation des images. Pourquoi faire cela&#x202F;? Nous allons le voir, Tropy permet d'enregistrer systématiquement des informations sur les droits d'utiisation des images d'un corpus donné, anticipant une future mise en ligne ou une réutilisation quelconque des ressources enregistrées dans un projet. C'est ainsi une occasion de sensibiliser les chercheurs et chercheuses aux subtilités, voir la complexité, de la réutilisation des images dans un contexte de recherche dont les modalités ne sont pas toujours connues. En France, l'Institut national d'histoire de l'art a rendu disponible un guide pratique pour la recherche et la réutilisation des images d’&oelig;uvres d’art <!-- fournir lien interne, le document est sous licence libre et peut être fourni par PH -->. Toutefois, selon les specificités de vos sources, il faut pas négliger de rechercher et d'enregistrer les informations propres à vos sources concernant leur réutilisation et possibilité de partage. 

Nous allons vous fournir trois possibilités pour travailler avec le jeu de données de votre préférence et selon  le degré de familiarité que vous avez aux techniques d'acquisition de ressources numériques.       

### Présentation du corpus d'images: les affiches de Mai 68
Nous allons découvrir comment travailler avec Tropy en utilisant un corpus d'images numérisées disponibles en ligne sur le site de [Gallica](http://gallica.bnf.fr/), la bibliothèque numérique de la Bibliothèque nationale de France (ci-après BnF) et de ses institutions partenaires. Notre corpus se compose d'environ quatre cents affiches numérisées de [Mai 1968 en France](https://fr.wikipedia.org/wiki/Mai_68). Ces affiches, à l'origine des [sérigraphies](https://fr.wikipedia.org/wiki/S%C3%A9rigraphie) pour la plupart, ont été principalement des créations du dit [Atelier populaire de l'Ecole des Beaux-Arts](https://www.persee.fr/doc/mat_0769-3206_1988_num_11_1_403852) de Paris lors de l'occupation de cette école en mai-juin 1968, mais aussi d'ateliers de lutte du même type qui se sont constitués dans d'autres villes (Montpellier, Marseille...). Plusieurs bibliothèques et musées disposent des bribes des affiches de Mai 68 dans leurs collections, toutefois Gallica donne accès à une collection numérisée quasi-complète qui rassemble des items physiquement présents dans diverses institutions. Ces numérisations datent des années 2010 et font partie des opérations en masse qui ont constitué le patrimoine numérique français à l'époque qui a suivi l'inauguration du projet de Google Library (aujourd'hui en berne). Elles témoignent aussi de la patrimonialisation de l'évènement de Mai 68 et de l'effet de celle-ci sur la création et mise à disposition de la source numérisée. Les fichiers images des affiches sont téléchargeables en format PDF ou JPEG depuis le site de Gallica. 

### Préparer son corpus d'images d'archives
Vous pouvez suivre cette leçon soit en utilisant le corpus des images d'affiches de Mai 1968 ou en privilégiant un corpus de votre préférence y compris vos propres images d'archives. Dans le premier cas, merci de suivre les instructions que nous fournissons sur comment obtenir ces fichiers. *(N.D.L.A. Ces instructions seront ajoutées une fois que le brouillon de la leçon aura intégré le jeu de données)*

Si vous préférez utiliser vos propres sources, n'hésitez pas à commencer avec le fruit d'une journée de travail au centre d'archives de votre préférence&#x202F;: des centaines de fichiers de photos en forme brute, que vous venez de copier depuis votre smartphone sur votre disque dur, sans même avoir eu le temps de les renommer, et qui attendent patiemment votre attention. C'est le moment de s'en occuper&#x202F;! 

### Les archives du Printemps érable 

[archives du mouvement du Printemps érable](https://www.printempserable.net/)

### Les photos d'Occupy Wall Street sur Flickr
        

 
## Installer Tropy 
Tropy peut être librement téléchargé depuis son [site web](https://tropy.org/). C'est un logiciel multi-plateformes (distributions Linux, Windows, macOS) dont l'installation se fait en local. Pour le moment, il n'existe pas d'application disponible en ligne, sachez donc que votre projet sera hébergé sur le disque dur de votre ordinateur. Il n'est pas non plus possible d'installer Tropy sur un serveur partagé pour travailler à plusieurs de manière synchrone.  

Notre leçon mobilise la version 1.14.0 de Tropy. Une fois le téléchargement terminé, lancez l'installateur et laissez-vous guider par les instructions.   

## Démarrer avec Tropy 
Cette section fournit les informations préalables à la création d'un projet qui vous permettra par la suite d'organiser les sources de votre projet de recherche.  

### Les éléments d'un projet dans Tropy 
Avant de commencer, il est important de comprendre les éléments de base qui structurent un projet dans Tropy. Ces éléments sont les suivants&#x202F;: 
* projet
* objet 
* liste
* *tag* (soit libellé)

De manière sommaire, un projet consiste en un ensemble d'objets qui peuvent être organisés en listes, mais aussi classés selon des libellés qui leur attribuent une caractéristique spéciale. 

Le *projet* est une collection de fichiers images qui représente une recherche localisée sur un sujet: une ébauche de publication, une initiative de crowdsourcing soit tout projet intellectuel susceptible d'englober un ensemble de sources captées en images que nous souhaitons analyser. Techniquement, le projet est le premier point d'entrée dans l'interface de Tropy, pour ensuite accéder aux photos d'archives qui lui correspondent afin de les organiser et d'effectuer de nombreuses opérations (transcription, prise de notes, indexation...) en vue de leur analyse. 

Passons à l'*objet* qui, dans Tropy, est essentiellement la représentation de notre source&#x202F;: la photo d'un document d'archives, d'un monument, d'une œuvre d'art, d'une affiche... Un objet équivaut à une ou plusieurs photos&#x202F;: par exemple, dans le cas d'un document d'archives de plusieurs pages, nous pouvons avoir des photos distinctes qui correspondent à chaque page. Lorsque nous créons l'objet qui correspond à ce document dans Tropy, nous le verrons, celui-ci englobe les photos de toutes les pages pour compter comme une unité.   

Ces objets nous pouvons ensuite les organiser en *listes*. Par liste, dans Tropy, il faut entendre une série, ou une sous-partie, que nous constituons en rassemblant plusieurs objets qui partagent une caractéristique commune selon la problématique de notre projet. Par exemple, si notre projet porte sur la création artistique d'une certaine période, nous pouvons constituer des listes selon les avant-gardes de la période en question ou selon artiste ou encore en appliquant des critères géographiques.   

Enfin, dernier mais non moins important élément de base, le libellé, ou &laquo;&#x202F;tag&#x202F;&raquo;. Il s'agit de mots-clés qui décrivent des caractéristiques distinctives d'un objet et permettent ainsi de le classer. Nous le verrons plus en détail par la suite, les tags sont des moyens d'[indexation personnelle](https://fr.wikipedia.org/wiki/Folksonomie) des objets que nous créons dans Tropy. Cette indexation peut être thématique ou fonctionnelle, à vous d'inventer le système qui vous convient mieux. Bien indexer nos sources au moment de les enregistrer peut parfois être jugé chronophage. En réalité, c'est du temps gagné que nous récupérons lors de l'analyse et de la rédaction en facilitant l'accès, de manière transversale, à des sources qui peuvent faire partie de différentes listes mais qui peuvent être réorganisées suivant une ou plus de caractéristiques communes. 

### Configurer un projet standard ou avancé
Au moment de créer un projet, il faut préalablement définir s'il est de type standard ou avancé - l'option par défaut étant le projet standard. Il s'agit là d'[une fonctionnalité disponible à partir de la version 1.13 de Tropy](https://tropy.org/blog/new-project-types-in-tropy-1-13). Mais de quoi s'agit-il exactement&#x202F;? 

Un projet standard, au moment de l'importation des fichiers des images, crée aussitôt des copies de ces images pour les stocker dans un répertoire spécifique de Tropy. L'avantage dans ce cas est que notre projet devient intégralement portable. Par exemple, en le copiant sur une clé USB et en l'important dans un autre environnement de travail que notre ordinateur habituel, nous pouvons le retrouver tel que nous l'avions laissé dans son environnement d'origine, et continuer à travailler dessus sans interruption. L'inconvénient d'un projet standard est cependant qu'il nécessite des machines performantes avec beaucoup de mémoire disponible, car les fichiers images sont des fichiers volumineux. 

De son côté, un projet avancé n'effectue pas de copies des images d'origine. Celles-ci ne sont donc pas stockées dans un répertoire intégré au projet, même si nous pouvons toujours les voir via l'interface de Tropy. Ici, comme il le faisait dans ses versions précédentes, Tropy établit des liens, que nous appelons des chemins, vers les répertoires que nous avons initialement choisi comme emplacement pour stocker nos fichiers. Par exemple, cet emplacement peut se trouver sur le disque dur de notre PC dans `Documents`. L'avantage des projets avancés est qu'ils sont légers, puisqu'ils ne contiennent que les données que nous ajoutons (structure de notre projet, notes, libellés, transcriptions...). En revanche, pour assurer la portabilité d'un projet avancé, il faudra veiller à l'accompagner, dans son nouvel environnement, des répertoires dans lesquels nous avons stocké nos images et d'intervenir pour rétablir les chemins cassés, le cas échéant. Si vous ne souhaitez pas mettre la main dessus ou ne savez pas trop comment s'y prendre, il vaut mieux sélectionner le mode standard, mais n'ayez pas peur de vous expérimenter plus tard.     
Pour suivre les étapes suivantes de la leçon, le choix de type de projet n'a pas vraiment d'incidence. En ce qui nous concerne, nous optons pour créer un projet avancé pour éviter d'avoir un projet lourd, mais, encore une fois, le choix vous appartient selon vos propres contraintes et préférences.

Admettons que nous avons créé notre projet, par défaut celui-ci est stocké dans le répertoire `Documents` et son extension est .TPY. Il est tout à fait possible de sauvegarder un projet Tropy à l'emplacement de notre préférence, que nous choisissons via la boîte de dialogue qui s'ouvre après avoir entré le nom de notre projet et appuyé sur le bouton `Create Project`. 
       
### Paramétrer la langue 
Tropy est disponible dans plusieurs langues dont le français. Pour paramétrer la langue à laquelle nous souhaitons rendre disponible l'interface, rendons-nous, à partir du menu principal, à `Édition` > `Préférences` > `Paramètres`. Une fois là, il est possible de sélectionner la langue de notre préférence à partir de la liste déroulante. Attention, la première fois que nous lançons Tropy le menu peut apparaître en anglais. Dans ce cas, suivre `Edit` > `Preferences` > `Settings` > `Locale` pour définir la langue de préférence.     

### Créer un projet
Lançons à présent Tropy - comme vous le verrez, nous avons aussitôt accès à une boîte de dialogue et aussi, en haut, au menu principal. La boîte de dialogue nous invite à créer un projet, d'abord en le nommant puis en sélectionnant son type&#x202F;: standard ou avancé - nous avons vu plus haut de quoi il s'agit [dans un moment](#configurer-un-projet). Nous pouvons aussi créer notre projet à partir du menu principal&#x202F;: `Fichier` > `Nouveau` > `Projet`. Nous n'allons pas explorer davantage le menu à ce point, sauf si nous souhaitons [paramétrer la langue de l'interface](#paramétrer-la-langue). 

Créons donc notre projet en lui attribuant le titre de notre préférence.

{% include figure.html filename="tropy-fr-01.jpg" alt="Capture d'écran de boîte de dialogue pour créer un projet dans Tropy" caption="Figure 1. La boîte de dialogue pour créer un projet dans Tropy" %} 

![Boîte de dialogue pour créer un projet dans Tropy](/images/tropy-fr-01.jpg "Figure 1. La boîte de dialogue pour créer un projet dans Tropy")


## Importer ses sources
Nous partons du principe que vous avez déjà des photos de vos archives ou que vous avez récupéré les fichiers que nous fournissons avec la leçon. Vous avez enregistré ces fichiers dans l'emplacement de votre choix sur votre disque dur.  

### Parcourir l'interface du projet 
Une fois notre projet créé et lancé, nous accédons enfin à l'interface qui permet d'effectuer les opérations globales le concernant&#x202F;: c'est l'interface du projet. L'autre interface principale via laquelle nous travaillerons est celle de l'objet, mais nous n'en sommes pas encore là&#x202F;! Restons pour le moment à l'interface du projet d'où nous avons accès au menu principal en haut&#x202F;; à un menu latéral à gauche qui offre un point supplémentaire d'accès à l'interface au projet, aux listes créées, mais aussi aux dernières importations que nous effectuons au fur et à mesure, tout comme aux tags et aux objets supprimés.  
<!-- ce qui suit n'est visible que si nous avons importé des fichiers- ici ce n'est pas le cas encore--> Depuis la zone du milieu, nous avons une vue d'ensemble des objets de notre projet et nous pouvons accéder à chacun d'eux pour les inspecter mieux et ce de deux façons. En plaçant le curseur de notre souris sur un objet, nous faisons afficher, dans le menu latéral à droite, des informations qui lui sont spécifiques&#x202F;: métadonnées, tags, le(s) fichier(s) de photo(s) qui se rapportent à cet objet. Cette zone du milieu offre un menu spécifique en haut qui permet notamment de naviguer dans les objets via une barre de recherche à droite - d'où aussi l'importance de [bien décrire les objets](#décrire-ses-sources) d'un projet&#x202F;! Autre fonctionnalité importante disponible dans ce menu&#x202F;: nous pouvons choisir si la vue d'ensemble des objets du projet s'affiche en mode liste ou en mode vignettes, en réglant le curseur, qui se trouve à gauche, de gauche à droite.   

### Importer les fichiers des images 
Il est possible d'importer les fichiers des images de deux façons. Soit les glisser, un par un ou en les sélectionnant tous, directement dans la zone du milieu du menu, réservée aux objets&#x202F;; soit utiliser le menu principal. Pour le faire depuis le menu, aller à `Fichier` > `Importer` > `Photos`, pour importer un ou plusieurs fichiers d’images depuis un répertoire; ou à Fichier > Importer > Dossier, si vous souhaitez importer tout un répertoire de fichiers. 

Les formats de fichiers que Tropy peut prendre en charge les principaux formats qui peuvent abriter des images dont JPG/JPEG, PNG, SVG, TIFF, GIF, PDF (pour une liste complète, se référer à la documentation du projet). 

### Importer des images depuis une page web
Il est possible d'importer des images statiques qui ont leur propre URL directement depuis une page web dans un projet Tropy. Pour ce faire, il faut se positionner dans l'interface du projet et glisser l'image sélectionnée depuis le navigateur vers la zone du milieu de l'interface offrant une vue d'ensemble des objets. Attention, l'importation est différente selon que le type du projet soit standard ou avancé. Si le projet est standard, Tropy effectue aussi une copie de l'image qui est ainsi téléchargée au cours de l'opération et intégrée dans le projet. En revanche, si le projet est en mode avancé, seulement un lien est créé vers l'adresse web de l'image, sans que celle-ci ne soit téléchargée. Dans ce cas, il faut soit double-cliquer sur l'objet créé dans notre interface pour accéder, via le web, à l'image d'origine soit effectivement la télécharger de son emplacement d'origine et la copier dans un répertoire sur notre disque dur pour ensuite l'importer dans le projet. 

Enfin, il faut noter que les opérations décrites ci-dessous sont possibles seulement avec les formats d'images statiques mais pas avec les fichiers PDF. Il faudra télécharger ces derniers pour ensuite pouvoir les intégrer dans iun projet Tropy. De même, lorsque les images sont accessibles via des pages dynamiques, comme le sont les pages générées via un moteur de recherche, il n'est pas possible de les importer directement dans Tropy. C'est en grande partie le cas d'images auxquelles nous accédons à la suite de recherches dans des bibliothèques numériques, et c'est aussi celui de notre corpus, que nous avons pris soin de télécharger afin de pouvoir l'utiliser. Comme bonne pratique, nous conseillons de télécharger et de sauvegarder en local les corpus qui constituent vos données de recherche.        

### Organiser, regrouper les images importées
Indépendamment de la manière dont vous avez importé vos photos, maintenant qu'elles sont bien là, essayez donc d'explorer à nouveau l'interface du projet. Vous pouvez ainsi régler l'affichage de vos photos dans la vue d'ensemble de la manière qui vous convienne le plus (en liste ou vignettes). Vous pouvez aussi vous placer sur un objet&#x202F;: en cliquant droit, vous avez accès à un menu supplémentaire permettant d'effectuer des opérations au niveau des objets. Au point où vous en êtes, vous pouvez utiliser ce menu pour, par exemple, tourner à gauche ou à droite des images, si cela est nécessaire. Notez que le click droit marche si vous êtes sur WIndows ou Linux&#x202F;; si vous êtes sur Mac, il faut maintenir la touche Ctrl enfoncée tout en cliquant (gauche) sur l'élément qui vous intéresse - un objet dans ce cas-ci.  

Vous pouvez aussi regrouper plusieurs fichiers de photos en un seul objet. Pourquoi faire cela&#x202F;? Peut-être que vous avez plusieurs photos qui se rapportent toutes à la même source primaire, par exemple six photos qui correspondent aux six pages d'un seul document. Dans ce cas, il ne s'agit pas d'objets distincts, puisque nous avons précisé qu'un objet est égal à une source primaire. Nous allons donc regrouper ces photos pour qu'elles correspondent à une seule source. <!--Ici ajouter un exemple inspiré du dataset utilisé pour la leçon--> 
Pour ce faire, Ctrl + cliquer pour choisir tous les fichiers concernés puis faire clic droit (ou la manipulation équivalente si vous êtes sur Mac) et choisir dans le menu qui s'ouvre `Fusionner les objets sélectionnés`. Lorsque vous faites la sélection des photos à regrouper, il faut commencer en cliquant d’abord sur le fichier qui
représente la première page du document puis à ceux qui suivent dans l'ordre souhaité. Alternativement, vous pouvez aussi glisser le fichier qui suit dans l'ordre sur le fichier qui sert d'entrée pour l'objet. Si un objet émane d’une fusion de fichiers, c'est le premier fichier qui hérite aux autres une série de caractéristiques, dont les métadonnées sont le plus important.          

## Décrire ses sources
Au moment d'importer les images de vos sources primaires, il est judicieux de décrire les fichiers avec les métadonnées d'origine des sources représentées. Cette opération va relier la photo avec la source et permettra ensuite son exploitation efficace (identifier les documents pour y accéder autant de fois qu'il le faut, les analyser, pouvoir les citer...). Merci de consulter la section qui suit avec des précisions sur les métadonnées, si ce mot vous semble étrange, autrement vous pouvez passer aux suivantes qui expliquent comment attribuer ces informations à nos objets.    

### Métadonnées: kézako? 
Avant toute chose, faisons, très brièvement, le point sur les métadonnées&#x202F;! Les métadonnées sont des informations qui décrivent d'autres données et qui deviennent signifiantes dans un système défini. Dans un cadre scientifique, comme le nôtre, [les métadonnées servent à décrire les données de recherche et les productions réalisées après leur analyse (par ex. articles, livres etc.)](https://doranum.fr/metadonnees-standards-formats/metadonnees-standards-formats-fiche-synthetique_10_13143_vbjs-6288/). Les métadonnées de base auxquelles nous avons affaire dans le cadre de notre projet peuvent porter sur le titre, le créateur ou la créatrice de la ressource qui nous intéresse (une oeuvre d'art, un document diplomatique), la date de création, parfois des destinataires ou encore davantage, comme nous le verrons plus en détail par la suite.      

### Attribuer des métadonnées par lot
Il est possible d'attribuer des métadonnées aux objets soit à l'unité soit par lot, si nos objets sont homogènes (par exemple, s'il s'agit d'un ensemble de photos de documents en provenance de la même archive, série et sous-série, carton...). C'est le cas de notre corpus, nous pouvons donc attribuer les principales métadonées, en tout cas celles qui sont communes, par lot. Pour ensuite attribuer, au niveau d'objet si besoin, des métadonnées spécifiques si elles ne sont pas communes pour l'ensemble. 

Une bonne pratique pour attribuer des métadonnées communes à un lot de photos est de se positionner au niveau de la dernière importation (accessible depuis le menu à gauche via l'interface du projet). Dans notre cas, la dernière importation est aussi notre importation originelle, mais il s'agit d'une bonne pratique à adopter. Au fil d'un projet, plusieurs importations de fichiers d'images peuvent se faire de manière différée, selon la temporalité d'une recherche, successivement à la suite d'une série de séjours dans différents centres d'archives... Cela veut dire qu'un projet peut s'étendre au fil du temps pour englober plusieurs importations de fichiers. Si des métadonnées sont attribuées après chaque nouvelle importation, il n'est pas nécessaire de revenir sur ces anciennes couches à nouveau, au contraire il vaut mieux les préserver de modifications fortuites. C'est pourquoi nous nous positionnons au niveau de la dernière importation. 

*(A ajouter: description comment attribuer de manière groupée des métadonnées avec aussi un exemple d'attribution de métadonnées plus spécifiques au niveau de l'objet en se rapportant à notre corpus d'affiches).* 
Depuis l'interface du projet, nous nous plaçons au niveau de la zone du milieu avec la vue d'ensemble des objets que nous avons importés. Nous les sélectionnons tous, que ce soit depuis l'affichage en mode liste ou vignette, Ensuite, nous accédons au menu qui se trouve dans la partie droite de notre écran pour aller à ce qui se présente comme une fiche `Métadonnées`. Pour le moment, cette boîte de dialogue est de type `Tropy Generic`, si nous nous fions à son intitulé - cela peut changer depuis la liste déroulante, mais restons là pour l'instant. Cette boîte comporte une liste de champs cliquables que nous pouvons peupler d'informations. Nous identifions comme informations communes à tous les objets de notre corpus les champs source, collection, droits. Nous allons donc renseigner chacun de ces champs. Les métadonnées sont appliquées à tous les objets sélectionnés. 

### Attribuer des métadonnées par objet
Nous allons maintenant travailler au niveau de l'objet. Nous venons d'[attribuer massivement des métadonnées](#attribuer-des-métadonnées-par-lot) qui sont communes à tous nos objets&#x202F;; à présent, nous souhaitons renseigner plus de métadonnées qui peuvent être spécifiques à un objet, comme par ex. un auteur ou la date de création. Nous pouvons le faire soit à partir de l'interface du projet, dans sa partie droite, que nous connaissons déjà, soit en accédant à l'interface de l'objet. Découvrons enfin cette dernière à laquelle il est possible d'accéder en double-cliquant sur l'objet de notre prédilection à partir de la liste ou de sa vignette. 

Une fois là, nous pouvons renseigner les champs pertinents à l'aide de la boîte de dialogue en haut à gauche, onglet `Métadonnées`. Si nous le souhaitons, nous pouvons d'ores et déjà indexer nos objets en insérant des tags pertinents à partir de la boîte de dialogue en haut à gauche, onglet `Tags`. 

### Personnaliser le modèle de saisie des métadonnées 
Pour se familiariser avec l'attribution de métadonnées à nos objets dans Tropy, nous avons utilisé jusqu'à présent le modèle générique de métadonnées embarqué. Tropy fournit deux modèles embarqués supplémentaires qui peuvent convenir à la description de la plupart des sources historiques. L'un de ceux-là est `Tropy Correspondence` qui peut servir soit tel quel soit légèrement personnalisé dans des cas de sources primaires qui sont des correspondances (lettres, correspondances diplomatiques...). L'autre modèle embarqué reproduit un format simple du standard (de fait) de métadonnées [Dublin Core](https://fr.wikipedia.org/wiki/Dublin_Core). <!--Ajouter ici davantage d'informations sur Dublin Core?--> Retenez ici seulement que, si les objets de votre projet Tropy ont vocation à être exportés puis importés et publiés dans un site web pour constituer une bibliothèque numérique, il s'agit fort probablement du modèle qu'il vous faut utiliser.   

Mais il est tout à fait envisageable de construire le modèle parfaitement adapté à vos sources, si vous n'avez pas peur de mettre un peu la main dans le cambouis. Dans ce cas, attention à ne pas essayer de tout construire à nouveau de fond en comble et rester dans l'esprit, ne serait-ce large, des champs déjà fournis lorsque vous apportez des adaptations. Pour personnaliser le modèle de saisie des métadonnées, voici la démarche à suivre. À partir du menu principal, aller à `Édition` > `Préférences` > `Modèle de saisie`. Dans le menu déroulant qui s'affiche, choisir puis dupliquer un modèle existant et nommer le modèle créé (par exemple, Affiches ou Monuments ou autre, selon l'objet d'une recherche donnée). Il est possible de renommer les champs existants à partir de `Label` ou, si besoin, d'ajouter de nouveaux champs.
*Ici à ajouter exemple avec le dataset de la leçon*. <!-- Ici ajouter une exemple de création de modèle de saisie selon le jeu de données mobilisé dans cette leçon -->  

## Analyser et annoter ses sources primaires 
          
### Organiser sa collection d'objets en listes 
Les listes permettent de regrouper les objets (des représentations de documents ou d'autres sources primaires) qui présentent une cohérence qu'elle soit thématique, chronologique ou autre en cohérence avec la problématique d'une recherche. Organiser ses objets en listes cohérentes peut faciliter considérablement l'analyse de ses sources puis leur mobilisation lors de la phase de l'écriture. Pour créer une liste, aller au menu principal de Tropy et sélectionner `Fichier` > `Nouveau` > `Liste`. Alternativement, depuis l'interface du projet, cela est possible depuis le menu latéral situé à gauche en faisant cliquant droit sur cette zone-ci et en choisissant `Nouvelle liste`. Nous voyons maintenant apparaître dans le menu latéral de gauche l'icône d'un répertoire et une boîte qu'il faut renseigner avec le nom de la liste. Par la suite, nous pouvons glisser un ou plusieurs objets (sélectionner les objets puis glisser via click droit) sur le nom de la liste pour les intégrer dans celle-ci. 

Il est tout à fait possible de créer des listes imbriquées pour organiser des parties et des sous-parties de votre travail. Il est à noter que la suppression d’une ou de plusieurs listes n’a pas d’incidence sur les objets qui eux
continuent d’exister dans le projet.

### Traiter et analyser un objet 
Nous avons vu plus haut comment [intégrer les informations descriptives qui nous aident à identifier nos sources](#décrire-ses-sources). Cette opération a normalement lieu dans la temporalité de l'importation des nos fichiers. A l'étape suivante, lorsque nous en sommes à travailler de plus près avec nos sources, nous avons la possibilité d'effectuer plusieurs types d'opérations. 

Tout d'abord, nous pouvons effectuer des opérations techniques de base pour améliorer la qualité de nos photos (régler la luminosité, le contraste, etc.) en se servant du menu qui se trouve en haut de la zone où s'affiche l'image. Il est possible aussi de zoomer sur une image pour mieux lire ou observer, d'inverser les couleurs pour, par exemple, lire plus facilement des microfilms. Ou encore, nous pouvons sélectionner une partie de l'image qui nous intéresse particulièrement et sauvegarder cette sélection, qui reste accessible depuis le menu latéral à gauche, pour y revenir aussi souvent que nécessaire. En outre, une sélection peut être sauvegardée en tant qu'image autonome avec ses propres métadonnées. Cela est possible en cliquant droit sur le nom de la sélection, depuis la zone du menu latéral gauche où elle apparaît, et choisir `Exporter la photo` dans le menu qui apparaît.  

Ensuite, nous avons la possibilité d'indexer le contenu de l'objet en ajoutant des tags. Les tags peuvent nous aider à organiser les contenus de nos sources de manière transversale à travers les listes. C'est un moyen très utile pour obtenir une vue latérale sur nos sources et facilite largement la rédaction. Notre conseil et de réfléchir en amont sur un système pertinent de mots-clés, selon la nature d'une recherche et sa problématique, et d'établir une liste à utiliser systématiquement. Cette liste peut bien sûr s'étendre au fil d'une recherche, elle permet néanmoins de se fixer sur de termes donnés en évitant leur multiplication, des formes différentes et des incohérences qui pourraient rendre finalement l'indexation moins efficace. 

Au dessous de la zone de l'image de l'objet, un éditeur de texte permet la prise de notes. Il est possible de créer autant de notes que souhaité, celles-ci apparaissent ensuite sous forme de liste tout en bas à gauche dans la zone du menu latéral gauche. La transcription du contenu d'une image, si celle-ci représente un texte, est aussi possible à faire sous forme de note. Tropy ne dispose pas de logiciel de reconnaissance optique de caractères intégré, par conséquent l'exportation automatique de texte à partir des images du projet n'est pas possible. 
Si l’objet a émané d’une fusion, les notes peuvent néanmoins s’insérer séparément pour chaque fichier. Les notes sont exportables soit via un export global du projet Tropy soit séparément en cliquant droit dessus et en choisissant de les exporter dans le menu qui s'affiche. 



## Extensions d'un projet Tropy
Il est possible d'exporter un projet Tropy à l'aide du menu principal en format JSON-LD ou PDF.  
Par ailleurs, une série de plugins peuvent être installés à l'aide du menu des préférences, ce qui permet d'exporter un projet aussi en format CSV. Si ce n'est pas l'objet de cette leçon, il mérité néanmoins d'évoquer la possibilité d'installer un plugin Omeka S qui permet d'exporter un projet pour le publier à l'aide d'un site web Omeka. <!-- Prévoir ici d'intégrer un lien pour la traduction française de la leçon sur Omeka en cours de préparation -->   

## Bibliographie
Les références bibliographiques rassemblées dans cette section sont principalement en français.  

### Généralités 
Mourlon-Druol, Emmanuel. &laquo;&#x202F;Déstructuration et restructuration de l’archive à l’ère numérique&#x202F;&raquo;. Billet de blog. Site web d'Emmanuel Mourlon-Druol https://www.e-mourlon-druol.com/. 7 novembre 2019. URL: [https://www.e-mourlon-druol.com/destructuration-et-restructuration-de-larchive-a-lere-numerique/](https://www.e-mourlon-druol.com/destructuration-et-restructuration-de-larchive-a-lere-numerique/), date de consultation 15 août 2024.

Gandanger, Aliénor et Valentine Gandanger. &laquo;&#x202F;Gazengel - Ooooh Tropy&#x202F;!&#x202F;&raquo;. 
Site web Luxembourg Centre for Contemporary and Digital History (C²DH). 22 février 2024 https://www.uni.lu/c2dh-fr/news/gazengel-ooooh-tropy/ 

Denoyelle, Martine et Johanna Daniel. Guide pratique pour la recherche et la réutilisation des images d’&oelig;uvres d’art 2021. Institut national d'histoire de l'art. [https://www.inha.fr/_resources/PDF/2021/2021_LIVRET_GUIDE-PRATIQUE_web_15062021.pdf](https://www.inha.fr/_resources/PDF/2021/2021_LIVRET_GUIDE-PRATIQUE_web_15062021.pdf)

### Tutoriels et ressources éducatives
Arènes, Cécile, Meriç Akdogan, & Aurélien Moisan. *Tropy , un outil pour gérer les corpus iconographiques*. Love Data Week Sorbonne Université. Zenodo. 17 février 2023 https://doi.org/10.5281/zenodo.7656554

Gérer ses photos de recherche avec Tropy. Tutoriel de l'atelier de formation de la Bibliothèque universitaire de l'université Rennes 2. Date de dernière mise à jour: 18 juillet 2024. [https://tutos.bu.univ-rennes2.fr/c.php?g=702342](https://tutos.bu.univ-rennes2.fr/c.php?g=702342).  

Laillier, Benjamin. *Tutoriel Tropy* (version 4), août 2019 http://doi.org/10.5281/zenodo.3381981 

<!-- le wiki est inaccessible
“Tropy | Gestion d’images”, wiki Pole-Num-Scrums-Skills, https://wikis.univ-lille.fr/proj-polnum/accueil/manuels/guide-d-utilisation-de-tropy
--> 

Valmalle, Delphine. &laquo;&#x202F;Utiliser Tropy pour la gestion de ses photos d'archives&#x202F;&raquo;. YouTube, *Geneatech*, 22 février 2021, https://youtu.be/AiPqbdwP67E  

<!-- en anglais “Tropy Webinar, June 16, 2020 (unedited recording)”, YouTube, Tropy Project, https://youtu.be/jWjP90EWHkQ --> 

## Notes 

[^1] Arlette Farge, *Le goût de l'archive*, Paris, Éditions du Seuil, 1989, 10.  

[^2] Frédéric Clavert, &laquo;&#x202F;Introduction&#x202F;&raquo; in Frédéric Clavert & Caroline Muller (dir.), *Le goût de l’archive numérique*,
https://gout-numerique.net/

[^3] Sean Takats, &laquo;&#x202F;Tropy&#x202F;&raquo;, billet de blog, _Quintessence of Ham_, 26 octobre 2017, http://quintessenceofham.org/2017/10/26/tropy date de consultation 1<sup>er</sup> septembre 2023

[^4] Ministère de la Culture, Département des études, de la prospective, des statistiques et de la documentation (DEPS). "Chiffres clés. Statistiques de la culture et de la communication 2022", p. 177-178. [URL](https://web.archive.org/web/20240104142707/https://www.culture.gouv.fr/Thematiques/Etudes-et-statistiques/Publications/Collections-d-ouvrages/Chiffres-cles-statistiques-de-la-culture-et-de-la-communication-2012-2022/Chiffres-cles-2022) 
