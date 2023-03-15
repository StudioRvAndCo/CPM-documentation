# Rapport de Projet Cinéma Project Manager
Equipe :
- Wagner Samy
- Verrier Martin
- Chiotti Maël
- Canin Corentin
## Sommaire :

- Introduction
    - Présentation de Studio Rv & Co
    - Présentation de Cinema Project Manager
    - Cahier des charges de CPM
- Équipe
    - Gestion de projet
    - Outils utilisés (CI/CD, trello …)
- Conception
    - Maquette
    - Base de données
- Technologies
    - Front-end
    - Back-end
- Conclusion
    - Difficultés rencontrées
    - État du projet actuel

## Introduction
### **Présentation de Studio Rv & Co**

Studio Rv & Co est une association à but non lucratif produisant divers projets audiovisuels comme des courts-métrages, des séries ou des talk shows. Elle compte une quinzaine de membres, dont Bastien Moirez-Charron qui est le tuteur de ce projet.

En activité depuis 2018, le collectif produit chaque année des projets de plus en plus ambitieux. C’est pourquoi, ce qui se faisait autrefois sur une semaine, nécessite désormais le travail de plus en plus de personnes tout au long de l’année. Ainsi, cette augmentation d’effectifs et de charge de travail implique inévitablement un besoin d’organisation interne. En effet, les documents finissent par se multiplier (scénarios, plannings, découpages techniques, listes des intervenants et leurs rôles…), cela devient un problème qu’il est nécessaire de résoudre.

### **Présentation de Cinema Project Manager**

Afin de continuer son bon fonctionnement et son développement, l’association a donc besoin d’un outil de gestion de projets. Néanmoins les solutions existantes sur le marché ne sont pas adaptées à la taille de l’association. Les outils sont soit trop peu développés (pour les petits indépendants), soit trop complexes (pour les gros studios de production). Ainsi, le studio Rv & Co a pris la décision de créer leur propre gestionnaire.

Cinéma Project Manager a donc été imaginé par Maël et Maxime, deux membres de l'association, pour leur projet de DUT. L’objectif de cet outil est de centraliser les différentes ressources utiles à Rv & Co pour la production d’un projet : découpages techniques, intervenants, plannings, lieux de tournage et plus.
Ainsi, cet outil doit permettre à chaque membre de l’association de paramétrer des projets, et de consulter son avancement.

### **Cahier des charges de CPM**

L'outil doit donc être disponible sur ordinateur, pour faciliter la création et le paramétrage de projets, mais également sur téléphone pour la consultation sur les lieux de tournage.

L'application doit fournir un système d'authentification, afin d'éviter de rendre public des informations privées.

En effet, l'application doit permettre l'enregistrement et la consultation de :

- Nom, prénom, numéro de téléphone des membres.
- Nom et lien Map des localisations de tournages.
- Titre, description, date de début, date de fin, nombre de plans, plans tournés, liste des épisodes et type d'un projet.
- Numéro, titre, description, nom du directeur, nombre de plans, plans tournés, ainsi que la liste des séquences d'un épisode.
- Numéro, titre, description, date de début, date de fin, nombre de plans, plans tournés, ainsi que la liste des plans d'une séquence.
- Numéro, valeur, description, état d'avancement (tourné ou non) d'un shot.

D'autre part, l'application doit être responsive, afin de s'adapter à tout type de téléphone et Desktop.


## Equipe

### **Gestion de projet**

Notre équipe avait la particularité de compter trois membres de Studio Rv & Co (Corentin, Maël et Samy) dont deux ayant déjà une expérience de tournage avec l’association. D'autre part, Martin, bien que ne faisant pas partie de l’association, a très vite assimilé les concepts importants.

De ce fait, nous connaissions parfaitement les besoins de l’association et nous pouvions facilement imaginer quelles fonctionnalités sont importantes pour l’application, mais aussi lesquelles sont prioritaires. En effet, l’objectif étant lors de ce projet de constituer une base solide, qui sera ensuite reprise par l’association, il a été important pour nous de savoir prendre des décisions sur les fonctionnalités à implémenter lors de ce projet. De plus, nous avons eu besoin d’anticiper les futurs besoins de l’association, pour orienter le développement de CPM, de telle sorte à faciliter la reprise du projet par la suite.

Ainsi, notre travail a commencé par une phase de conception logicielle et graphique sur laquelle nous avons travaillé tous les quatre, ce qui a mené à la création d’une maquette d’interface utilisateur répondant aux fonctionnalités prioritaires souhaitées pour CPM.

Ensuite, nous nous sommes naturellement répartis les tâches selon les préférences de chacun : Martin a pris en main le back-end avec Samy en renfort sur la fin du projet. Quant à Maël, Samy et Corentin, ils ont développé le front-end.

### **Outils utilisés**

En ce qui concerne la communication au sein du groupe, nous avons utilisé la plateforme Discord. Nous l'utilisons pour communiquer entre les membres de l’équipe mais également avec Bastien, notre tuteur, pour que celui-ci nous fasse des retours sur l’avancement de notre projet.

Par ailleurs, afin d’avoir un suivi des tâches à réaliser, en cours et terminées, nous avons utilisé un tableau Trello, comme suit :

 ![Tableau Trello](https://cdn.discordapp.com/attachments/1064484713407987712/1085668322537914560/1AapdOG5zOoWUAjC3Qd9VD_ss18SVdt_ULNyZzGbJDvjZYfyA0Uh377SLQE8bvAY.png "Tableau Trello")

 _Cet outil nous a permis de visualiser le travail des membres de l’équipe en temps réel, et d'organiser au mieux les différents spring._

D’autre part, nous avons mis en place quatre dépôts Git dans l’organisation GitHub de l’association. Deux pour le back-end et deux pour le front-end avec à chaque fois un dépôt “sandbox” pour nous permettre d’expérimenter les technologies (surtout au début) et un dépôt principal.
Chacun de ces dépôts comportaient une branche main, une branche dev et des actions GitHub de formatage automatique du code afin de garantir le respect des conventions d’écriture. La branche main est la branche contenant la dernière version stable de l’application. Lorsque nous ajoutions une fonctionnalité, nous passions toujours par la branche dev.
De plus, afin de garantir la stabilité des branches lors des merges, nous avons mis en place des Pull Request. En effet, lors d’une demande de merge, une revue de code de la part d’un autre membre était systématiquement demandée. Ce qui nous a permis un meilleur contrôle de la qualité de nos ajouts.
Enfin, pour ne pas perdre trop de temps sur des problèmes mineurs, nous avons utilisé le système d’Issues pour garder une trace des améliorations à réaliser mais non prioritaires. En effet, comme nous l’avons précédemment expliqué, ce projet à vocation à être récupéré et continué par les membres de l’association. Ainsi garder une trace des améliorations est essentiel.

## Conception

### **Maquette**

Une fois les principales fonctionnalités définies, nous nous sommes attelés à la création d’une maquette qui nous permettrait de mieux imaginer l’interface graphique. Nous avons commencé par proposer des idées sur tableau noir pour avoir une première idée rudimentaire de ce que nous voulions. Nous nous sommes d’abord concentré sur l’interface mobile car celle-ci présente plus de contraintes que l’interface Desktop.

![Première maquette](https://cdn.discordapp.com/attachments/1064484713407987712/1085669244475277352/14t_UCyGuLklY9eSBOS84dHi8p4MnlYnSAJWUq1-kY1pcoLoJIx2DJF2tBH7tS4k.png "Première maquette")

_Exemple des maquettes qui ont été réalisées sur tableau_

Nous sommes ensuite passés à l’outil de création de maquettes interactives en ligne Figma. Cet outil nous a permis de construire des maquettes bien plus complètes et bien plus proches de ce que nous allions développer ensuite, une sorte de modèle à suivre lors du développement :

![Maquette Figma Mobile](https://cdn.discordapp.com/attachments/1064484713407987712/1085669274510708908/12RjD8jB0a6EP4SGz1AzxCf4GDqlU6MbVIgeTTm_HIP9axtStA4ce1qw-hSag6qQ.png "Maquette Figma Mobile")

![Interface Mobile](https://cdn.discordapp.com/attachments/1064484713407987712/1085669307117215844/14BOTUev7OVuqfvihoFLSmAgebEz6JALTeYiTVsXnyYkv5c5YkegPILIyXNvguw.png "Interface Mobile")

_Comparaison entre une vue sur la maquette Figma et sur l’application_

À partir de cette interface mobile, nous avons construit l’interface Desktop, tirant profit de la plus grande surface d’affichage du support.

![Maquette Figma Ordinateur](https://cdn.discordapp.com/attachments/1064484713407987712/1085669355368493076/1vjhbxHsn-cOb4JIHaAKmxaGeYIEjdrNBaLTb9Hdq-5FXtbHV6pKvUZYjxcfH9A.png "Maquette Figma Ordinateur")

_Interface Desktop conçue sur Figma_

### **Base de données**

Connaissant les fonctionnalités de notre application, ainsi que sa maquette, qui permettra de guider le développement du frontend. Nous avons dû établir la base de données que nous allions implémenter, afin de guider le développement du backend.

Pour ce faire, nous avons dû dans un premier temps, définir le type de base de données que nous souhaitions utiliser. Pour ce choix, plusieurs facteurs sont entrés en compte, pour prendre la décision d’implémenter une base de données NoSQL mongoDB.

Dans un premier temps, cette technologie a été choisie par un membre de l’association. De plus, le NoSQL apporte un avantage de performance dans notre cas d’utilisation. En effet, dans le cadre de gestion d’un projet, l’utilisateur peut être amené à modifier des données. Ces modifications peuvent porter sur un projet complet, mais aussi et surtout, sur des petits éléments. Ainsi, lorsque l’utilisateur modifie un simple élément d’un projet, le NoSQL est plus performant que le SQL.
En NoSQL, nous pouvons modifier, et récupérer des sous éléments de document JSON, alors qu’en SQL nous devrions manipuler les tables entières à chaque requête.

Ainsi, nous avons mis en place une base de données mongoDB qui comporte 4 collections :
- User : comporte toutes les informations de connexion des utilisateurs
- Location : comporte toutes les informations sur les localisations de tournages
- Member : comporte toutes les informations sur les membres de l’association
- Project : comporte toutes les informations des différents projets de l’association.

## Technologies utilisées
### **Front-end**

Pour répondre à la contrainte multi-plateforme du projet, nous avons choisi de développer l’application front-end en Flutter.
Flutter est un SDK développé par Google depuis 2017. Flutter permet de créer facilement des interfaces graphiques grâce à un système de widget similaire à ce que nous connaissions avec Java Swing, avec l’avantage supplémentaire de permettre la compilation sur la majorité des plateformes (Windows, MacOS, Linux, Android, iOS et Web) car il est rédigé en Dart, un langage orienté objet développé lui aussi par Google et prévu pour la compilation multi-plateformes.

Bien que nous découvrions Flutter et Dart avec ce projet, la prise en main fut facile et rapide grâce notamment à l'excellente documentation disponible en ligne. On peut noter également que nous avons essayé au mieux de respecter la convention de design Material Design 3 de Google avec notre application, ce qui fut facilitée par la prise en charge d’une majorité de composants et paramètres de Material Design 3 nativement dans Flutter.

Lorsque l’on développe avec Flutter, il faut parfois faire attention à certaines spécificités des plateformes disponibles. Par exemple, certaines fonctionnalités relatives au transfert de fichiers depuis le stockage pourraient être accessibles sur Desktop ou Mobile, mais pas en web. Il faut donc trouver des alternatives pour contourner ces limitations.

### **Back-end**

Pour communiquer avec la base de données et établir le backend de CPM, nous avons choisi de continuer sur la base fournie par l’association, utilisant C# et ASP.NET. ASP.NET est le framework web intégré à la plateforme .NET de Microsoft, open source et multiplateforme depuis 2016, et permet de développer une API pouvant être auto-générée par Swagger en langage C#. L’avantage d’ASP.NET est d’être un framework spécifiquement dédié au web, particulièrement robuste et disposant d’un support important à la fois par Microsoft et de nombreux contributeurs open source. Il est ainsi un choix judicieux et moderne pour une API web qui pourrait avoir à supporter une lourde charge si CPM venait à se développer à une large échelle.

## Conclusion

### **Difficultés rencontrées**

Nous avons dû évidemment découvrir de nouvelles technologies pour ce projet. En ce qui concerne le front-end, l’apprentissage de Flutter prit un petit temps d’adaptation, notamment pour assimiler comment organiser les widgets et les contenir pour obtenir un résultat responsif. Il fallut également comprendre comment inclure de la logique au sein des widgets pour les rendre moins statiques et qu’ils s’adaptent au contexte (la solution étant le constructeur de widgets Builder). Pour ce qui est du backend, en plus du temps d’adaptation au NoSQL, qui est un concept que nous n’avions pas eu l’occasion de rencontrer dans notre programme, nous avons rencontré des difficultés avec le driver C# pour mongoDB afin d’établir les différentes routes API.


### ***État du projet actuel***

L’application est actuellement prête pour constituer une première version utilisable en tournage. Il est possible d’ajouter, modifier et supprimer des membres et des lieux de tournage ainsi que des projets. Il reste cependant du développement à effectuer, afin d’arriver au niveau prévu par la maquette.
Notre objectif avec Flutter était de proposer, pour un même code source, une interface différente selon le support, plus adaptée au format d’affichage. Nous avons cependant abandonné cette idée par manque de temps et nous avons préféré nous concentrer sur l’interface Mobile, car plus adaptée au format Desktop que l’interface Desktop n’est adaptée au format Mobile mais surtout car elle est à la base de l’interface Desktop.


## Glossaire

**Cinema Project Manager (CPM)** : Application de gestion de projets audiovisuels de l’association Studio Rv & Co.

**Studio Rv & Co** : Association de production audiovisuelle porteuse du projet CPM.

**Projet** : Production audiovisuelle (film ou série).

**Séquence** : Portion d’un projet définie par une unité de lieu

**Plan** : Portion d’une séquence correspondant à une image entre deux coupes au montage.

**Flutter** : SDK d’interface utilisateur open-source de Google.

**Dart** : Langage de programmation orienté objet de Google spécialisé dans la création d’applications

**MongoDB** : Système de gestion de base de données orienté documents de la mouvance NoSQL.

**Mobile** : Plateformes à modalité d’interaction tactile au format d’affichage proche de celui d’un smartphone (smartphones et tablettes Android ou iOS, navigateurs web sur Android ou iOS).

**Desktop** : Plateformes au format d’affichage proche d’un écran d’ordinateur avec interaction clavier souris (ordinateurs sous Windows, macOS, Linux, navigateurs web sur ordinateur).

**Material Design** : Convention de design proposée par Google pour les interfaces graphiques d’applications et logiciels.

**Figma** : Outil de conception d’interface graphique.

**Trello** : Outil de gestion de projets.