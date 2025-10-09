---
title: Analyse des besoins - Présentation générale
---

# Présentation du projet

## Méthodologie pour la cueillette des données
- Rencontre d’équipe : discussion initiale pour définir la vision générale du projet, les attentes et les fonctionnalités principales
- Brainstorming : échange collectif permettant d’identifier les besoins des étudiants, les fonctionnalités clés et les problèmes liés au processus d’inscription aux cours

## Description du domaine

### Fonctionnement
Le système est basé sur une architecture client–serveur:
- Le frontend (HTML, CSS, JavaScript) offre une interface qui permettant aux étudiants de naviguer facilement dans la plateforme et interagir avec les fonctionalités principales
- Le backend (Java / Spring Boot) assure la logique, la gestion des requêtes et la communication entre le frontend et la base de données ;
- La base de données (PostgreSQL) stocke les cours, les utilisateurs et les avis
- Le serveur Nginx utilisé comme proxy inverse pour diriger les requêtes entre le frontend et le backend, tout en aidant à sécuriser les échanges.
- L’application est déployée sur un serveur Ubuntu 22.04 LTS.


### Acteurs
| Acteur | Rôle principal | Objectifs |
|-------------|--------------------|----------------|
| Étudiant utilisateur | Utilisateur principal du système | Consulter les cours, s’inscrire ou se désinscrire, consulter ou publier des avis sur les cours et enseignants. |
| Professeurs / Auxiliaires d’enseignement | Fournisseurs d’information pédagogique | fournissent les plans de cours et mettent
à jour les informations en lien avec un cours|
| API| Source de données | Fournir les données officielles relatives aux cours, aux horaires et aux inscriptions |
| Discord | Plateforme de communication externe | Faciliter les échanges entre étudiants et consultation des avis sur les cours |


### Dépendances
- Backend : Spring Boot 
- Frontend : HTML, CSS, JavaScript
- Serveur : Ubuntu 22.04 LTS
- Serveur web : Nginx


## Hypothèses et contraintes

TODO: Liste des hypothèses de travail et des contraintes (techniques, organisationnelles, etc.).



