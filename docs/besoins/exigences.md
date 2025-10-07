---
title: Analyse des besoins - Exigences
---

# Exigences

## Exigences fonctionnelles
- [ ] EF1 : L'étudiant peut s'inscrire à la plateforme avec ses identifiants UdeM
- [ ] EF2 : L'étudiant peut se connecter à la plateforme
- [ ] EF3 : L'étudiant peut personaliser son profil
- [ ] EF4 : L'étudiant peut rechercher des cours par son code pu son titre
- [ ] EF5 : L'étudiant peut consulter les informations complètes d'un cours (horaire, professeur, plan de cours, etc)
- [ ] EF6 : Le système permet d'afficher les avis étudiants après un mimimum de 5 avis
- [ ] EF7 : Le système permet à un étudiant de soumettre un avis à propos d'un cours via Discord
- [ ] EF8  : Le système permet à l'étudiant de mettre des cours dans son panier et de s'y inscrire ainsi que s'y désinscrire 
- [ ] EF9 : L'étudiant peut comparer plusieurs cours
- [ ] EF10 : L'étudiant peut accéder à son horaire 
- [ ] EF11 : Le système centralise dans une interface les données de Planifium et des avis Discord 

## Exigences non fonctionnelles

TODO: Contraintes de performance, sécurité, compatibilité, etc.


- [ ] ENF1 : Interface simple et claire pour tous les étudiants
- [ ] ENF2 : Compatible avec les navigateurs (Firefox, Google, Safari)
- [ ] ENF3 : Aucune données personelle identifiable (conformité Loi 25)


## Priorisation

TODO: Identifier les exigences critiques.

### Exigences Critique
- EF1: Authentification (Accès sécurisé à la plateforme)
- EF2 : Connexion à la plateforme
- EF4 : Recherche de cours
- EF6 : Affichage des avis 
- EF8 : Gestion du panier 
- EF9 : Compaison des cours
- EF11 : Centralisation des données
- ENF1 : Interface utilisateur
- ENF3 : Confidentialité

##  Exigences secondaire
- EF3 : Profil personnel
- EF7 : Soumission d'avis
- EF10 : Consultation horaire
- ENF2 : Compatibilité avec les navigateurs




## Types d'utilisateurs

> Identifier les différents profils qui interagiront avec le système.

| Type d’utilisateur | Description | Exemples de fonctionnalités accessibles |
|--------------------|-------------|------------------------------------------|
| Utilisateur non authentifié | Accès limité sans connexion | Consultation basique des cours, recherche simple |
| Utilisateur authentifié | Utilisateur connecté | Recherche, gestion du panier, soumission avis, comparaisons de cours |
| Administrateur | Gestionnaire de la plateforme | Création/suppression de ressources, gestion des utilisateurs, gestion des données|

<!-- TODO: Détailler selon le périmètre du projet. -->

## Infrastructures

> Informations sur l’environnement d’exécution cible, les outils ou plateformes nécessaires.

- Le système sera hébergé sur un serveur Ubuntu 22.04.
- Base de données : PostgreSQL version 15.
- Serveur Web : Nginx + Gunicorn (pour une app Python, par exemple).
- Framework principal : Springboot
