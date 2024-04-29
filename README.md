Système de Réservation de Billets
    1. Introduction:
Ce projet présente un système de gestion de théâtre basé sur le Web et développé à l'aide de Flask, MySQL et HTML/CSS. Le système est conçu pour rationaliser les opérations d'un cinéma, en fournissant des fonctionnalités aux caissiers et aux gérants pour gérer efficacement les projections de films, les réservations et la vente de billets.

But et objectifs :
L'objectif principal de ce projet est d'automatiser et d'améliorer la gestion d'un théâtre, en facilitant des interactions fluides entre les clients, les caissiers et les gérants. Les objectifs du projet comprennent :

1. Gestion efficace des réservations :
Permettez aux clients de voir les projections de films disponibles, de sélectionner des sièges et d'effectuer des réservations en ligne.
  
2. Ventes de billets rationalisées :
Fournissez aux caissiers une interface conviviale pour traiter les ventes de billets, gérer les réservations et gérer efficacement la disposition des sièges.
  
3. Gestion complète du spectacle :
Donnez aux gestionnaires les moyens de planifier des projections de films, d'attribuer des salles et de superviser le prix des billets en fonction de facteurs tels que le type de film et le jour de la semaine.
  
4. Gestion de la base de données :
Implémentez un schéma de base de données robuste pour stocker et gérer les données essentielles liées aux films, aux horaires, aux salles, aux réservations et aux tarifs.

 

    2. Aperçu du projet:
       
Description du projet:
Le système de gestion de théâtre est une application Web développée pour moderniser et rationaliser les opérations d'un théâtre. Il facilite diverses fonctionnalités tant pour les clients que pour le personnel du théâtre, notamment la réservation de billets, la gestion des spectacles et les tâches administratives.

Fonctionnalité et caractéristiques :
1.Authentification utilisateur :
Les utilisateurs sont authentifiés en fonction de leurs rôles (caissier ou manager) et ont accès aux fonctionnalités respectives.
  
2. Réservation de billets :
Les clients peuvent consulter les projections de films disponibles, sélectionner des sièges et réserver des billets pour les séances souhaitées.
  
3. Gestion du spectacle :
Les gestionnaires peuvent planifier des projections de films, attribuer des salles et gérer les tarifs en fonction du type de film et du jour de la semaine.
  
4. Disposition des sièges :
Le système fournit une représentation visuelle de la disposition des sièges dans les différentes salles, permettant aux utilisateurs de sélectionner des sièges pendant le processus de réservation.
  
5. Gestion de la base de données :
Utilise la base de données MySQL pour stocker et gérer les données liées aux films, aux horaires des séances, aux salles, aux réservations et aux prix.

Technologies utilisées :
- Flask : framework web Python utilisé pour développer la logique backend et le routage.
- MySQL : système de gestion de bases de données relationnelles utilisé pour le stockage et la gestion des données.
- HTML/CSS : langages frontaux utilisés pour concevoir des interfaces utilisateur et des mises en page.

Public cible:
Le public cible du système de gestion de théâtre comprend :

    • Clients:
Personnes souhaitant réserver des billets de cinéma en ligne et accéder à des informations sur les projections de films.


    • Caissiers :
Personnel du théâtre chargé du traitement de la vente des billets, de la gestion des réservations et du traitement des demandes des clients.
    • Gestionnaires :
Personnel administratif chargé de planifier les projections de films, d'attribuer les salles et de superviser les stratégies de tarification.

L'application répond aux besoins des clients recherchant une expérience de réservation pratique et du personnel du théâtre nécessitant des outils efficaces pour gérer les opérations du théâtre.



    3. Architecture du système:
Aperçu:
Le système de gestion de théâtre suit une architecture client-serveur, où l'interface côté client est implémentée à l'aide de HTML/CSS et la logique côté serveur est développée à l'aide de Flask. Le système interagit avec une base de données MySQL pour stocker et gérer les données essentielles liées aux films, aux horaires des séances, aux salles, aux réservations et aux tarifs.

Architecture client-serveur :
Le système suit une architecture client-serveur, où :
    • Client : fait référence à l'interface frontale accessible par les utilisateurs (clients, caissiers et gestionnaires) via les navigateurs Web.
    • Serveur : fait référence au serveur backend implémenté à l'aide de Flask, qui gère les demandes des clients, traite les données et communique avec la base de données.

Interactions front-end et back-end :

Front-End (HTML/CSS) :
L'interface frontale est chargée de présenter l'interface utilisateur aux clients, y compris les formulaires de connexion, les pages de réservation, les listes de spectacles et les outils de gestion. Il interagit avec le serveur back-end en envoyant des requêtes HTTP (POST/GET) basées sur les actions de l'utilisateur, telles que la soumission de formulaires ou les clics sur des boutons.
  
Back-End (Flacon) :
Le framework Flask est utilisé pour développer la logique backend de l'application. Il définit des itinéraires pour gérer les demandes entrantes du client, traite les données, effectue des opérations de logique métier et restitue des modèles HTML dynamiques pour générer des réponses. Le back-end communique avec la base de données MySQL pour récupérer ou manipuler des données en fonction des demandes des utilisateurs.

Schéma de base de données :
Le schéma de base de données MySQL joue un rôle crucial dans le système en stockant et en gérant diverses entités et leurs relations. Le schéma comprend des tables telles que « films », « spectacles », « salles », « booked_tickets » et « price_listing », qui stockent des informations sur les films, les horaires, la disposition des sièges, les réservations et les stratégies de tarification. Les relations entre les tables sont établies à l'aide de contraintes de clé étrangère pour garantir l'intégrité et la cohérence des données.

Le schéma de base de données sert d'épine dorsale du système, fournissant un référentiel centralisé pour le stockage et la récupération des données essentielles aux opérations de gestion du théâtre.



    4. Caractéristiques:
1. Authentification de l'utilisateur :
- Description:
Les utilisateurs sont authentifiés en fonction de leurs rôles (caissier ou gestionnaire) à l'aide d'un nom d'utilisateur et d'un mot de passe.
- Contribution:
Cette fonctionnalité garantit un accès sécurisé aux fonctionnalités du système, permettant uniquement aux utilisateurs autorisés (caissiers et gestionnaires) d'effectuer les opérations pertinentes.

2. Réservation de billets :
- Description:
Les clients peuvent consulter les projections de films disponibles, sélectionner des sièges et réserver des billets pour les séances souhaitées.
- Contribution:
Permet aux clients de réserver facilement des billets de cinéma en ligne, rationalisant ainsi le processus de billetterie et améliorant l'expérience utilisateur.


3. Gestion du spectacle :
- Description:
Les gestionnaires peuvent planifier des projections de films, attribuer des salles et gérer les tarifs en fonction du type de film et du jour de la semaine.
- Contribution:
Fournit aux gestionnaires des outils pour organiser et gérer efficacement les projections de films, optimiser l'utilisation des salles et mettre en œuvre des stratégies de tarification dynamiques pour maximiser les revenus.

4. Disposition des sièges :
- Description:
Le système fournit une représentation visuelle de la disposition des sièges dans les différentes salles, permettant aux utilisateurs de sélectionner des sièges pendant le processus de réservation.
- Contribution:
Améliore l'expérience utilisateur en offrant une interface conviviale pour la sélection des sièges, réduisant ainsi la confusion et les erreurs pendant le processus de réservation.

5. Gestion de la base de données :
- Description:
Utilise la base de données MySQL pour stocker et gérer les données liées aux films, aux horaires des séances, aux salles, aux réservations et aux prix.
- Contribution:
Sert de référentiel centralisé pour stocker les données essentielles, garantissant l'intégrité, la cohérence et la récupération efficace des données pour des opérations de gestion de théâtre transparentes.

Caractéristiques uniques ou innovantes :
- Tarification dynamique:
Le système met en œuvre une tarification dynamique basée sur des facteurs tels que le type de film et le jour de la semaine, permettant aux gestionnaires d'ajuster les prix des billets pour optimiser les revenus.
- Disponibilité des sièges en temps réel :
Les clients peuvent consulter la disponibilité des sièges en temps réel et sélectionner des sièges en fonction de leurs préférences, offrant ainsi une expérience de réservation transparente et interactive.


Contribution globale :
Les fonctionnalités contribuent collectivement à la fonctionnalité globale de l’application en fournissant une solution complète pour la gestion du théâtre. De la réservation simplifiée des billets à la gestion efficace des spectacles et à la tarification dynamique, l'application vise à améliorer l'expérience globale du théâtre pour les clients et le personnel du théâtre.


    5. Conception de base de données :
Schéma de base de données :
Le schéma de base de données se compose de plusieurs tables interconnectées via des relations. Chaque table répond à un objectif spécifique : stocker et gérer les données liées aux films, aux horaires des séances, aux salles, aux réservations et aux tarifs.

Tableaux et colonnes :
1. films :
- Colonnes : movie_id, movie_name, length, language, show_start, show_end
- Objectif : stocke des informations sur les films, notamment leurs titres, leur durée, leur langue et les dates de début/fin de l'émission.

2. montre :
- Colonnes : show_id, movie_id, hall_id, type, time, Date, price_id
- Objectif : Enregistre les détails des projections de films, tels que le film, la salle, l'heure et la date, ainsi que les prix associés.

3. salles :
- Colonnes : hall_id, class, no_of_seats
- Objectif : contient des informations sur les salles, y compris leurs identifiants, leur classe (par exemple, or ou standard) et le nombre de places disponibles.

4. billets_réservés :
- Colonnes : ticket_no, show_id,seat_no
- Objectif : stocke les données concernant les billets réservés, y compris les numéros de billets, les identifiants de spectacle associés et les numéros de siège.

5. liste_de prix :
- Colonnes : price_id, type, jour, prix
- Objectif : Gère les détails des prix en fonction du type de film (par exemple, 2D, 3D) et du jour de la semaine.

6.types :
- Colonnes : movie_id, type1, type2, type3
- Objectif : définit les types de films pour chaque film, permettant une catégorisation basée sur des attributs tels que 2D, 3D ou 4DX.

Niveau de normalisation :
Le schéma de base de données présente un niveau de normalisation pour minimiser la redondance des données et garantir l'intégrité des données. Spécifiquement:
- Première Forme Normale (1NF) :
Tous les tableaux ont des valeurs atomiques dans chaque colonne et il n'y a pas de groupes répétitifs.
- Deuxième Forme Normale (2NF) :
Tous les attributs non clés dépendent entièrement de la clé primaire, sans dépendances partielles.
- Troisième Forme Normale (3NF) :
Il n'y a pas de dépendances transitives et tous les attributs non clés dépendent uniquement de la clé primaire.

La conception de la base de données adhère à ces principes de normalisation, ce qui donne lieu à un schéma bien structuré qui organise et maintient efficacement la cohérence des données.


    6. Détails d'implémentation:
Itinéraires des flacons :
    • Les itinéraires sont définis pour l'authentification des utilisateurs, la réservation de billets, la gestion des spectacles et d'autres fonctionnalités.
    • Chaque route traite les requêtes HTTP, interagit avec la base de données et renvoie les réponses appropriées.
Logique:
    • La logique métier est mise en œuvre pour gérer l'authentification des utilisateurs, la réservation de billets, la programmation des spectacles et la gestion des tarifs.
    • Des mécanismes de validation des données et de gestion des erreurs sont incorporés pour garantir la fiabilité du système.


Bibliothèques et API :
    • Le projet s'appuie principalement sur Flask pour le développement backend et MySQL pour le stockage des données.
    • Les interactions frontend sont gérées à l'aide de HTML/CSS et JavaScript.



    7. Essai:
Processus de test :
L'application a subi des tests rigoureux pour garantir sa fonctionnalité, sa fiabilité et sa sécurité. Le processus de test comprenait les éléments suivants :

1. Tests unitaires :
Les composants et fonctions individuels ont été testés isolément pour vérifier leur exactitude et leur fonctionnalité.

2. Tests d'intégration :
Différents modules et composants ont été intégrés et testés ensemble pour garantir une interaction et une fonctionnalité transparentes.

3. Tests d'acceptation des utilisateurs (UAT) :
De vrais utilisateurs, y compris des clients et du personnel du théâtre, ont été impliqués dans les tests de l'application afin de valider sa convivialité et son expérience utilisateur.

4. Tests de sécurité :
L'application a été soumise à des tests de sécurité pour identifier et corriger toute vulnérabilité ou menace, telle que l'injection SQL et le cross-site scripting (XSS).

Défis rencontrés :
Lors des tests, certains défis ont été rencontrés, notamment :
- Assurer la compatibilité entre les différents navigateurs Web et appareils.
- Résoudre les cas extrêmes et gérer les scénarios exceptionnels avec élégance.
- Assurer la cohérence et l'intégrité des données dans les opérations de bases de données complexes.

Résolution:
Pour relever ces défis, des procédures de tests approfondies ont été suivies et tous les problèmes identifiés ont été rapidement résolus grâce à un développement et un débogage itératifs. Des tests de compatibilité ont été effectués sur plusieurs navigateurs et appareils pour garantir une expérience utilisateur cohérente.


    8. Conclusion :

Résumé:
En conclusion, le projet a réussi à développer un système complet de réservation de billets de cinéma qui s'adresse à la fois aux clients et au personnel du cinéma. L'application fournit une interface conviviale pour réserver des billets, gérer des spectacles et administrer efficacement les opérations du théâtre.

Succès:
Le projet a atteint ses objectifs consistant à améliorer l'expérience cinématographique des clients, à rationaliser les processus de réservation de billets et à fournir aux gestionnaires de salles des outils permettant une planification efficace des spectacles et une gestion des prix. L'utilisation de technologies Web modernes, telles que Flask et MySQL, a facilité le développement d'une solution robuste et évolutive.

Améliorations futures :
Bien que la version actuelle de l'application réponde aux exigences de base, plusieurs domaines pourraient être améliorés à l'avenir, notamment :
- Mise en œuvre d'options avancées de sélection de sièges, telles que les préférences de siège et les aménagements spéciaux.
- Amélioration de l'interface utilisateur avec des fonctionnalités et des éléments visuels plus interactifs.
- Intégration avec des API externes pour des fonctionnalités supplémentaires, telles que des critiques de films et des recommandations.
- Implémentation de fonctionnalités avancées d'analyse et de reporting pour la gestion du théâtre.

Dans l'ensemble, le projet pose une base solide pour un développement et une amélioration ultérieurs, avec le potentiel d'évoluer vers une plateforme complète de gestion de salle de cinéma.


