# [](#header-1)Rapport de Stage - 02/06 au 11/08

Le stage effectué les deux derniers mois s'est déroulé au sein du Ministère de l'Intérieur, dans l'immeuble Lumière situé au cœur du douzième arrondissement de Paris. Ce lieu, non loin de Bercy Village, est un endroit où il est agréable de se rendre chaque matin. L'édifice, composé de huit étages et de quatre sous-sols, est un des plus grands immeubles de bureaux de Paris. Ses ascenseurs panoramiques aux allures futuristes et ses escalators de part et d'autre font rêver au premier coup d’œil. 
  
A mon arrivée, j'ai retrouvé mon tuteur qui m'a tout d'abord montré mon bureau ainsi que mes nouveaux collègues. Comme vous pouvez le voir sur l'organigramme, je faisais parti du BCA, le Bureau de la Conception Applicative, lui-même se trouvant dans la Sous-Direction des Applications. 


La SDA (Sous-direction des Applications) est en charge :
* du pilotage des projets applicatifs jusqu’à la vérification du service régulier (assistance à maîtrise d'ouvrage, étude et estimation des solutions techniques, conception, développement, tests et intégration)
* du pilotage des moyens opérationnels affectés aux projets (budget des projets, préparation et suivi des marchés)
* de la maintenance ''projet'' (corrective ou adaptative, évolutive en appliquant le processus projet)

Cette entité comprend environ cent trente agents, répartis en cinq bureaux :
* Bureau du Pilotage Applications (BPA)
* Bureau de la Conception Applicative (BCA)
* Bureau des Applications Métiers (BAM)
* Bureau des Applications Transverses (BAT)
* Bureau des Tests et de l'Intégration (BTI)


Le BCA (Bureau de la Conception Applicative) (relation client) est, au sein de la SDA, le bureau composé des métiers amont du cycle de vie du projet (l'assistance à la maîtrise d'ouvrage, la conception, l'architecture applicative, le développement, le support projet des bases de données, la gestion des référentiels et des composants).

Il compte environ trente personnes, réparties en trois sections : ''Assistance à maîtrise d'ouvrage'', ''Conception, Architecture, Référentiels'', ''Solutions et Développement''
  
 
  <img src="DSIC Organigramme.jpg" alt="Organigramme" style="width: 800px; display: block; margin: auto"/>
  
  
Après avoir fait la connaissance des nombreuses personnes travaillant autour de moi, j'ai pu rejoindre mon lieu de travail pour installer le matériel. 

La prise en main de mon système d'exploitation commencée (Ubuntu 16.04 LTS), j'ai pu explorer cette nouvelle interface, apprendre les commandes de base du Terminale et effectuer l'installation des composants nécessaires pour mon travail. 


## [](#header-2)Githug - 1ère semaine

  <img src="Githug-Logo.jpg" alt="Githug Screenshot" style="width: 200px"/>

A l'aide d'un tutoriel de mise en pratique des connaissances théoriques, appelé Githug et écrit en Ruby, j'ai approfondi mes connaissances concernant les commandes de Terminale de Git (git revert, git diff, git bisect etc.), et possède désormais de solides bases utiles tout au long de ma scolarité.
  
    
  <img src="Githug Screenshot.png" alt="Githug Logo" style="width: 600px; display: block; margin: auto;"/>


Git est un logiciel de gestion de versions décentralisé, permettant à plusieurs développeurs de travailler sur un même projet et d'avoir un suivi des modifications. Il est possible pour chaque utilisateur de développer sur son propre dépôt, de manière décentralisé, en évitant ainsi certains conflits entre les fichiers.

  <img src="https://f.hypotheses.org/wp-content/blogs.dir/3252/files/2017/03/basic-remote-workflow-git.png" alt="Githug Logo" style="width: 600px; display: inline-block; margin: auto;"/>  


## [](#header-2)Docker - 2ème et 3ème semaine 

  <img src="docker-logo.png" alt="Logo Docker" style="width: 200px"/>

Le premier outil sur lequel j'ai du travaillé s'intitule Docker. Il s'agit d'un logiciel libre permettant la mise en oeuvre de conteneurs s'exécutant en isolation, via une API de haut-niveau. Ce dernier utilise les fonctionnalités du noyau Linux et contrairement à une VM, il ne dispose pas de système d'exploitation. Le conteneur s'instancie grâce à une image Docker, regroupant un système de fichiers et un ensemble de paramètres. 

  <img src="VMS-Docker.jpg" alt="VMS vs Docker" style="width: 500px; display: block; margin: auto"/>
  
Un des avantages notables d'un conteneur Docker, en comparaison à une machine virtuelle, est son faible poids étant donné que ce dernier ne dispose pas d'OS, ce qui permet un lancement plus rapide et une migration facile. Aussi, il est possible de containériser une application, avec pour chaque couche des conteneurs isolant ses composants. Ce concept d'architecture de microservices est très utile du côté de la production.

  <img src="Dockerfile-Screenshot.png" alt="Dockerfile Screenshot" style="width: 600px; display: block; margin: auto"/>

L'utilisation de conteneurs s'opére grâce à un Terminale à l'aide de commandes diverses, même si ce dernier dispose dorénavant d'une interface graphique.
J'ai donc d'abord appris comment constuire un conteneur ainsi que tous les éléments nécessaires à son fonctionnement. Ensuite, j'ai réalisé un conteneur pour le développement de l'application que je devais réaliser.


## [](#header-2)Symfony 3 - De la 4ème à la 7ème semaine

Il est le 2ème outil sur lequel il m'a été donné de travaillé. 

Symfony est à la fois un assemblage de composants PHP et un framework open source en PHP, développé par des informaticiens français de SensioLabs et à destinations d'autres développeurs.

Il permet de travailler de façon plus structurée et rigoureuse (aménagements structurants définis par le squelette de tout projet Symfony) et plus rapidement (réutilisation de modules). 
Il facilite aussi la maintenance à long terme et l'évolutivité en proposant dès la conception un ensemble de normes de développement. Il fournit un contexte de développement complet avec un outil de debug.


#### [](#header-4)Arborescence

Son arborescence est ainsi organisé:
* Le dossier *app*    : configurations de l'application, traductions, templates etc
* Le dossier *bin*    : fichiers exécutables (ex: bin/console)
* Le dossier *src*    : code source de l'application, organisé en bundles
* Le dossier *var*    : fichiers générés (cache, logs, etc.)
* Le dossier *web*    : fichiers publics accessibles (css, js, images etc.)
* Le dossier *tests*  : liste des tests unitaires et fonctionnels
* Le dossier *vendor* : dépendances tiers de l'application


#### [](#header-4)MVC

L'architecture de Symfony 3 respecte l'architecture MVC (Modèle - Vue - Contrôleur), qui permet de séparer les différentes parties du code d'une manière logique.

Le contrôleur gère la dynamique de l'application. Elle fait le lien entre l'utilisateur et le reste de l'application.
Le modèle encapsule la logique métier ainsi que l'accès aux données. Il peut s'agir d'un ensemble de fonctions (Modèle procédural) ou de classes (Modèle orienté objet).
La vue s'occupe des interactions avec l'utilisateur : présentation, saisie et validation des données.

Cette manière d'organiser le code permet une meilleure conception du logiciel et notamment un gain de temps dans sa maintenance. Cependant, cela implique trois fois plus de fichiers et une architecture plus complexe.

#### [](#header-4)Bundles

Un bundle est une brique d’une application, un répertoire qui contient tout ce qui concerne une fonctionnalité donnée. Cela permet de bien organiser les différentes parties d’un site. 
Un des avantages de cette découpe en bundles est la possibilité de partager à la communauté les bundles réalisés, ou alors de les réutiliser dans une autre application, voir même d'utiliser des bundles développés par d'autres utilisateurs (des exemples connus tels que FOSUserBundle, FOSRestBundle etc).

Il s'organise d'une manière bien précise, avec un dossier Controller où l'on déposera nos contrôleurs avec la convention de nommage suivante: *nomcontroleurController*. On trouve aussi un dossier Entity où sont stockés tous nos modèles. Et enfin un dossier Resources est également présent, avec des sous-dossiers *config* (fichiers de configuration du bundle), *public* (fichiers js, css, img etc), *views* (vues de notre bundle).


## [](#header-2)Drupal 8 - De la 8ème à la 11ème semaine

