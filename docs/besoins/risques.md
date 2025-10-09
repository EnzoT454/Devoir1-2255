---
title: Analyse des besoins - Risques
---

# Analyse des risques

## Identification des risques


### Risque 1 – Données insuffisantes pour les avis

- **Probabilité** : Élevée
- **Sévérité** : Moyenne 
- **Impact** : Si un nombre restreint d’étudiants fournit des retours, la plateforme manquera de crédibilité et de pertinence.
- **Plan de mitigation** :  
  - Promouvoir la participation sur Discord
  - Mettre en avant des statistiques visuelles pour inciter les étudiants à contribuer
  - Autoriser les retours anomymes pour augmenter la participation

### Risque 2 - Confidentialité des étudiants
- **Probabilité** : Moyenne 
- - **Sévérité** : Élevé 
- **Impact** : Risque de divulgation d'informations personnelles si les données ne sont pas bien gérées.  
- **Plan de mitigation** :  
  - Ne jamais stocker de noms avec des avis
  - Anonymiser tous les messages avant leurs enregistrement
  - Consultation avec le bureau de conformité de l'UdeM

### Risque 3 - Diversité des expériences
- **Probabilité** : Élevée
- **Sévérité** : Moyenne
- **Impact** : Les avis peuvent varier selon le profil des étudiants (internationaux, début de parcours, fin de parcours, 1er cycle, 2e cycle), ce qui peut engendrer de la confusion. 
- **Plan de mitigation** :  
  - Filtres personalisés qui permet de voir les avis par profil similaire
  - Ajouter un indicateur de fiabilité associé à chaque ensemble d'avis, basé sur le nombre de retours et la diversité des participants 

### Risque 4 - Dépendance aux données officielles
- **Problème** : externe (dépendance aux sources de données)
- **Probabilité** : Moyenne  
- **Sévérité** : Moyenne 
- **Impact** : Une indisponibilité ou une mise à jour tardive de Planifium ou des résultats académiques limiterait la fiabilité du système.
- **Plan de mitigation** :  
  - Mettre en place une sauvegarde locale des données Planifium
  - Ajouter une fonction de mise à jour manuelle pour les administrateurs

### Risque 5 – Fiabilité et performance du système
- **Problème** : interne (architecture et charge du système)
- **Probabilité**  : Moyenne
- **Sévérité** : Élevée
- **Impact** : Si le serveur subit des ralentissements (lenteur des appels API, surcharge, erreurs de connexion), les utilisateurs peuvent abandonner la plateforme, réduisant ainsi son adoption.
- **Plan de mitigation** :
  - Mettre en place un cache local pour éviter d’appeler trop souvent l’API Planifium.
  - Effectuer des tests de charge avant la mise en ligne.

## Modification du processus opérationnel

> Si la mise en place du système modifie des processus internes ou des pratiques actuelles, il est essentiel de les identifier ici.

L'intégration de Discord comme principale source d'avis change la façon dont les étudiants recueillent et partagent les informations sur les cours. Au lieu que les étudiants doivent chercher des avis un peu partout, tout sera maintenant centralisé sur une même plateforme

Ce changement implique : 
- Une meilleure gestion de la confidentialité afin de proteger l'identité des étudiants 
- Une dépendance à Discord pour obtenir des avis récents et variés
- Un suivi régulier pour garder les informations à jour et représentative aux cours chercher