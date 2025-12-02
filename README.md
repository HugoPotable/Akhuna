# AKHUNA

### Open Source Sports Coaching Ecosystem

> 🚀 **[ACCÉDER À LA PRÉSENTATION INTERACTIVE ET AU WBS GRAPHIQUE](https://ton-pseudo.github.io/ton-repo/)**
> *Ce tableau de bord interactif présente la vision, la structure détaillée et la roadmap du projet.*

---

## PROJECT ABSTRACT

**Akhuna** est une solution open-source alternative aux plateformes propriétaires de coaching sportif. Conçue pour briser le verrouillage technologique, elle offre aux entraîneurs une gestion complète et gratuite : planification, analyse de performance et feedback vidéo. Reposant sur une architecture web et mobile modulaire, Akhuna garantit la souveraineté des données et permet un développement communautaire extensible.

---

## WORK BREAKDOWN STRUCTURE (WBS)

Ce découpage structure le développement pour une équipe de 7 ingénieurs sur 24 mois, couvrant l'intégralité du cycle de vie logiciel.

### 1. PROJECT MANAGEMENT & METHODOLOGY
* **Pilotage Stratégique :** Définition de la roadmap, planification des sprints (Agile/Scrum) et gestion des risques.
* **Reporting Académique :** Suivi des KPIs de vélocité, rapports d'avancement (Follow-ups) et préparation des soutenances.
* **Tooling :** Configuration et maintenance de l'environnement de gestion (Jira, GitHub Projects, Notion).

### 2. UX/UI DESIGN & CONCEPTION
* **Recherche Utilisateur :** Analyse des besoins, rédaction des User Stories et définition des flux utilisateurs (User Flows).
* **Design System :** Création de l'identité visuelle et d'une bibliothèque de composants (UI Kit) cross-platform pour assurer la cohérence.
* **Prototypage :** Maquettes haute-fidélité (Figma) pour les interfaces Web (Espace Coach) et Mobile (Espace Athlète).

### 3. BACKEND ARCHITECTURE & INFRASTRUCTURE
* **Infrastructure as Code :** Déploiement des environnements (Dev/Staging/Prod), orchestration (Docker) et gestion de la base de données.
* **Core API Gateway :** Développement des microservices critiques (Authentification JWT, Gestion des droits RBAC).
* **Services Métiers :** API de gestion des programmes d'entraînement et service de traitement des médias (compression/stockage S3).

### 4. WEB CLIENT DEVELOPMENT (COACH SPACE)
* **Architecture Frontend :** Initialisation du framework SPA (React/Vue), gestion du routing et du state management global.
* **Program Builder :** Module complexe d'édition de planning (Drag & Drop, cycle de périodisation, duplication).
* **Dashboard CRM :** Interfaces de visualisation de données (Data viz) et gestion administrative des athlètes.

### 5. MOBILE CLIENT DEVELOPMENT (ATHLETE SPACE)
* **Architecture Mobile :** Setup de l'environnement cross-platform (React Native/Flutter) et gestion du mode offline-first.
* **Training Player :** Interface d'exécution de séance temps-réel (Chronos, Inputs de performance, RPE).
* **Feedback Loop :** Système de capture et d'upload vidéo asynchrone pour analyse technique par le coach.

### 6. QUALITY ASSURANCE & DEVOPS
* **CI/CD Pipelines :** Automatisation des tests, du linting et du déploiement continu via GitHub Actions.
* **Testing Strategy :** Écriture des tests unitaires (Backend), d'intégration et tests E2E (Parcours critiques).
* **Documentation :** Rédaction de la documentation technique, API Reference (Swagger) et guides de contribution open-source.

---

## FUNCTIONAL SPECIFICATIONS (HIGH-LEVEL)

Description technique des systèmes majeurs définis dans le WBS.

**Core Infrastructure & Backend System**
Le cœur du système repose sur une API centralisée et sécurisée, conçue pour la scalabilité. Ce module gère l'authentification et les permissions granulaires (Coach vs Athlète). Il assure la persistance et l'intégrité des données sportives complexes (séries, répétitions, charges, historique) et orchestre les interactions entre les clients via des endpoints RESTful optimisés. Il inclut un service dédié au stockage et au streaming des fichiers médias (vidéos de correction).

**Coach Interface (Web Platform)**
Outil de productivité principal, cette interface Web (SPA) permet la conception macro et micro-cyclique des entraînements. Elle intègre un moteur de visualisation de données avancé pour analyser la progression des athlètes sur le long terme. Le module "Program Builder" offre une expérience riche (type IDE) pour la création rapide de plans complexes.

**Athlete Interface (Mobile Application)**
Application compagnon native focalisée sur l'expérience utilisateur en situation de mobilité (salle de sport). Elle remplace le carnet d'entraînement physique en permettant la saisie intuitive des scores et des métriques physiologiques. Elle assure la synchronisation bidirectionnelle des données avec le serveur (support offline) et facilite la communication multimédia avec le coach.

**Quality & Deployment Pipeline**
En tant que projet open-source, ce module transverse garantit la robustesse et la maintenabilité du code. Il comprend l'automatisation complète des processus de validation (CI) et de livraison (CD) pour permettre des itérations rapides sans régression. Il inclut également la production d'une documentation technique exhaustive indispensable pour l'onboarding de nouveaux contributeurs communautaires.