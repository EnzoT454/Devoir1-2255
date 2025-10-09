---
title: Analyse des besoins - Exigences
---

# Exigences

## Exigences fonctionnelles
- [ ] EF1 : L'étudiant peut s'inscrire à la plateforme avec ses identifiants UdeM
- [ ] EF2 : L'étudiant peut se connecter à la plateforme
- [ ] EF3 : L'étudiant peut personaliser son profil
- [ ] EF4 : L'étudiant peut rechercher des cours par son code ou son titre
- [ ] EF5 : L'étudiant peut consulter les informations complètes d'un cours (horaire, professeur, plan de cours, etc)
- [ ] EF6 : Le système permet d'afficher les avis étudiants après un mimimum de 5 avis
- [ ] EF7 : L'étudiant peut comparer plusieurs cours
- [ ] EF8 : Le système centralise dans une interface les données de Planifium, des avis Discord anisi que les résultats académiques 

## Exigences non fonctionnelles



- [ ] ENF1 : Interface simple et claire pour tous les étudiants
- [ ] ENF2 : Compatible avec les navigateurs (Firefox, Google, Safari)
- [ ] ENF3 : Aucune données personelle identifiable (conformité Loi 25)


## Priorisation


### Exigences Critique
- EF1: Authentification (Accès sécurisé à la plateforme)
- EF2 : Connexion à la plateforme
- EF4 : Recherche de cours
- EF6 : Affichage des avis 
- EF8 : Gestion de la section de comparaison
- EF9 : Comparaison des cours
- EF11 : Centralisation des données
- ENF1 : Interface utilisateur
- ENF3 : Confidentialité

##  Exigences secondaire
- EF3 : Profil personnel
- ENF2 : Compatibilité avec les navigateurs




## Types d'utilisateurs

> Identifier les différents profils qui interagiront avec le système.

| Type d’utilisateur | Description | Exemples de fonctionnalités accessibles |
|--------------------|-------------|------------------------------------------|
| Utilisateur non authentifié | Accès limité sans connexion | Accès à la page d'inscription |
| Utilisateur authentifié | Utilisateur connecté | Recherche, personalise profil, comparaisons de cours |
| Administrateur | Gestionnaire de la plateforme | Création/suppression de ressources, gestion des utilisateurs, gestion des données|


## Infrastructures

> Informations sur l’environnement d’exécution cible, les outils ou plateformes nécessaires.

- Le système sera hébergé sur un serveur Ubuntu 22.04.
- Langage principal : Java
- Frontend : HTML, CSS et JavaScript
- Base de données : PostgreSQL version 15.
- Serveur Web : Nginx 
- Framework principal : Springboot
