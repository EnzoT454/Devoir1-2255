---
title: Conception - Architecture
---

# Architecture du système

## Vue d’ensemble

### Description du type d’architecture retenue :  
Le système CoursAdvisor adopte une architecture en couches orientée services **REST**.
Il s’agit d’un système web distribué composé de trois principaux conteneurs (frontend, backend et base de données) interagissant via des API HTTP REST et des échanges de données au format JSON.
L’application communique également avec des services externes tels que l’API Planifium (pour les informations de cours) et Discord (pour la centralisation des avis étudiants).  
### Raisons du choix :  
  - Permet une séparation claire des responsabilités (présentation, logique métier, données).
  - Facilite l’évolutivité (possibilité de modifier un module sans impacter les autres).
  - Compatible avec les intégrations externes (API Planifium et Discord).  

## Composants principaux  

- Interface (frontend)  
- Backend (Java)  
- Base de données  
- API Planifium (externe)  
- Discord (externe)  
- Profs/ auxiliaires (externe)

## Communication entre composants

- Mécanismes d’échange : appels HTTP, requetes SQL.
- Format des données : JSON, CSV.

## Diagramme d’architecture (Modèle C4)

### Diagramme d’architecture - Niveau 1
![Diagramme d’architecture - Niveau 1](./C4_niveau1.png)

---
### Diagramme d’architecture - Niveau 2
![Diagramme d’architecture - Niveau 2](./C4_niveau2.png)