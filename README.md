# AKHUNA

### Open Source Sports Coaching Ecosystem

> 🚀 **[ACCÉDER À LA PRÉSENTATION INTERACTIVE ET AU WBS GRAPHIQUE](https://hugopotable.github.io/Akhuna/)**
> *Ce tableau de bord interactif présente la vision, la structure détaillée et la roadmap du projet.*

---

## PROJECT ABSTRACT

**Akhuna** est une plateforme open-source destinée au coaching sportif moderne. Elle vise à remplacer les solutions propriétaires en offrant une alternative gratuite, modulaire et souveraine, couvrant la planification, le suivi de performance et l'analyse vidéo. Conçue pour être extensible par la communauté, elle s'appuie sur une architecture web et mobile robuste permettant une évolution continue du produit.

---

## WORK BREAKDOWN STRUCTURE (WBS)

Ce découpage structure le développement pour une équipe de 7 ingénieurs sur 24 mois, couvrant l'intégralité du cycle de vie logiciel.

### 1. PROJECT MANAGEMENT & METHODOLOGY
* **Pilotage Stratégique :** Définition de la roadmap, planification des sprints (Agile/Scrum) et gestion des risques.
* **Reporting Académique :** Suivi des KPIs de vélocité, rapports d'avancement (Follow-ups) et préparation des soutenances.
* **Tooling :** Configuration et maintenance de l'environnement de gestion (Jira, GitHub Projects, Notion).

### 2. UX/UI DESIGN & CONCEPTION
* **Recherche Utilisateur :** Interviews, analyse des besoins réels des coachs/athlètes, création de personas et définition des parcours utilisateurs.
* **Design System :** Définition d'un langage visuel complet incluant UI Kit, tokens (typographie, couleurs, espacements) et règles d'accessibilité.
* **Prototypage :** Production de maquettes haute fidélité dans Figma pour web et mobile, servant de référence pour les équipes de développement.

### 3. BACKEND ARCHITECTURE & INFRASTRUCTURE
* **Infrastructure as Code :** Définition et automatisation des environnements (Dev/Staging/Prod), conteneurisation et orchestration.
* **Core API Gateway :** Mise en place des services critiques (authentification, permissions, gestion des comptes) et normalisation des endpoints.
* **Services Métiers :** Gestion des programmes d'entraînement, traitement des médias (compression, stockage, streaming) et logique métier centrale.

### 4. WEB CLIENT DEVELOPMENT (COACH SPACE)
* **Architecture Frontend :** Structure SPA, routing, gestion d'état et intégration cohérente avec l'API.
* **Program Builder :** Outil avancé de création de programmes incluant drag & drop, périodisation et duplication intelligente.
* **Dashboard CRM :** Vue unifiée des athlètes, data visualisation et outils de gestion administrative.

### 5. MOBILE CLIENT DEVELOPMENT (ATHLETE SPACE)
* **Architecture Mobile :** Application cross-platform, gestion du mode hors-ligne et synchronisation fiable avec le backend.
* **Training Player :** Exécution guidée des séances avec chronos, consignes, interactions et saisies de performance.
* **Feedback Loop :** Capture vidéo, upload asynchrone et mise à disposition pour analyse technique par les coachs.

### 6. QUALITY ASSURANCE & DEVOPS
* **CI/CD Pipelines :** Automatisation complète de la validation, du build, des tests et des déploiements.
* **Testing Strategy :** Tests unitaires, intégration, E2E et validation continue des parcours critiques.
* **Documentation :** Rédaction de la documentation technique, guides contributeurs et référence API.

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