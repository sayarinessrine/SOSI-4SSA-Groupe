# SOSI – Application de gestion de la santé et du bien-être

## 1. Présentation du projet

**SOSI** est une application dédiée à la gestion et au suivi de la santé et du bien-être. Elle vise à faciliter l'accès aux services médicaux et à proposer différents services permettant aux utilisateurs de mieux gérer leur santé au quotidien.

Le projet est développé selon une **architecture microservices**, afin de séparer les fonctionnalités en services indépendants et faciliter leur maintenance et leur évolution.

## 2. Fonctionnalités principales

L'application SOSI est composée des modules suivants :

- **Gestion des utilisateurs :** inscription, authentification et gestion des profils.
- **Gestion du cycle menstruel :** suivi et gestion du cycle menstruel.
- **Gestion des services médicaux :** gestion des services et des rendez-vous médicaux.
- **Gestion de l'aide et des dons :** gestion des demandes d'aide et des dons.
- **Gestion du bien-être :** fonctionnalités liées au bien-être des utilisateurs.
- **Gestion des traitements et médicaments :** suivi des traitements et des médicaments.
- **Gestion de la communauté et des groupes de soutien :** échanges et interactions entre utilisateurs.

## 3. Architecture du projet

Le backend repose sur une architecture microservices. Chaque service possède une responsabilité spécifique.

Les principaux éléments de l'architecture sont :

- **Microservices Spring Boot :** gestion des fonctionnalités métier.
- **Microservice commun Symfony :** service commun développé avec Symfony.
- **API Gateway :** point d'entrée unique pour les requêtes du frontend.
- **Eureka :** découverte et enregistrement des services.
- **Keycloak :** gestion de l'authentification et des accès.
- **Bases de données :** PostgreSQL et/ou MongoDB selon les besoins de chaque service.

Les communications entre les services peuvent être synchrones (REST) ou asynchrones (événements).

## 4. Technologies utilisées

| Technologie | Utilisation |
|---|---|
| Spring Boot | Développement des microservices métier |
| Symfony | Développement du microservice commun |
| PostgreSQL / MongoDB | Gestion des données |
| Docker | Conteneurisation |
| Kubernetes | Orchestration des conteneurs |
| API Gateway | Gestion des requêtes entrantes |
| Eureka | Découverte des services |
| Keycloak | Authentification et autorisation |
| Swagger / Postman | Documentation et test des API |
| Git / GitHub | Gestion du code source et collaboration |

## 5. Organisation du dépôt

```text
SOSI/
│
├── Backend/
│   ├── SpringBoot/
│   │   ├── User-Service/
│   │   ├── Menstrual-Cycle-Service/
│   │   ├── Medical-Services-Service/
│   │   ├── Help-Donation-Service/
│   │   ├── Wellness-Service/
│   │   ├── Treatments-Medications-Service/
│   │   └── Community-Service/
│   │
│   ├── Symfony/
│   │   └── Common-Service/
│   │
│   └── Infrastructure/
│       ├── API-Gateway/
│       ├── Eureka/
│       ├── Docker/
│       └── Kubernetes/
│
├── Frontend/
│
├── Documentation/
│   ├── Presentation/
│   ├── Diagrams/
│   └── Document-Technique/
│
└── README.md
```

## 6. Gestion du projet

Le projet est réalisé en équipe. Chaque membre est responsable d'un ou plusieurs services selon la répartition des tâches définie par le groupe.

Le travail collaboratif est assuré à l'aide de Git et GitHub, avec une organisation du code source et un suivi des modifications.

## 7. État d'avancement

Le projet est actuellement en phase de conception et de préparation de l'architecture.

Les prochaines étapes comprennent :
- La conception détaillée des microservices.
- La définition des diagrammes de classes.
- La définition des contrats API et des interactions entre services.
- Le développement progressif des différents composants.
- Les tests et l'intégration des services.

---

**Projet académique – ESPRIT – Année universitaire 2026/2027**
