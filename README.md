<<<<<<< HEAD
# Template de projet REST API avec Javalin - IFT2255

Ce dépôt sert de template de base pour les projets REST API avec Javalin dans le cadre du cours IFT2255 – Génie logiciel.
Il fournit une structure organisée suivant une architecture MVC (Model–View–Controller) simplifiée, prête à être utilisée pour vos travaux.

## Structure du projet

```sh
rest-api/
│
├── src/
│   ├── main/
│   │   ├── java/com/diro/ift2255/
│   │   │   ├── config/
│   │   │   │   └── Routes.java           # Définition des routes HTTP
│   │   │   │
│   │   │   ├── controller/
│   │   │   │   ├── CourseController.java # Contrôleur pour les endpoints de cours
│   │   │   │   └── UserController.java   # Contrôleur pour les endpoints utilisateurs
│   │   │   │
│   │   │   ├── model/
│   │   │   │   ├── Course.java           # Modèle représentant un cours
│   │   │   │   └── User.java             # Modèle représentant un utilisateur
│   │   │   │
│   │   │   ├── service/
│   │   │   │   ├── CourseService.java    # Logique métier liée aux cours
│   │   │   │   └── UserService.java      # Logique métier liée aux utilisateurs
│   │   │   │
│   │   │   ├── util/
│   │   │   │   ├── HttpClientAPI.java    # Client HTTP pour appels externes
│   │   │   │   ├── HttpResponse.java     # Représentation d'une réponse HTTP
│   │   │   │   ├── HttpStatus.java       # Codes de statut HTTP
│   │   │   │   ├── ResponseUtil.java     # Outils pour formater les réponses
│   │   │   │   └── ValidationUtil.java   # Méthodes utilitaires de validation
│   │   │   │
│   │   │   └── Main.java                 # Point d’entrée du serveur Javalin
│   │   │
│   │   └── resources/                    # Ressources utilisées dans le code
│   │
│   └── test/                             # Tests unitaires (JUnit)
│
└── pom.xml
```

## Architecture

Ce template suit principalement le modèle MVC :

- **Model (`model/`)** : Représentation des entités du domaine (ex. User, Course)
- **Controller (`controller/`)** : Gestion des requêtes HTTP et appels au service
- **Service (`service/`)** : Logique métier centrale
- **Util (`util/`)** : Fonctions utilitaires réutilisables (validation, réponses, etc.)
- **Config (`config/`)** : Configuration du serveur et définition des routes
- **`Main.java`** : Point d’entrée du serveur (initialise Javalin et enregistre les routes)

## Bonnes pratiques

- Respectez la séparation des responsabilités entre **Controller**, **Service** et **Model**.
- Utilisez les classes du dossier `util/` pour les validations et la gestion des réponses HTTP.
- Centralisez les routes dans `config/Routes.java` pour simplifier l’ajout de nouveaux endpoints.
- Ajoutez des **tests unitaires** pour chaque méthode de service.
- Conservez un style de code uniforme (respect du standard Java).
=======


## CoursAdvisor (Brève description)
 
***CoursAdvisor*** est une plateforme web destinée aux étudiants du DIRO (Université de Montréal).
Elle centralise les données provenant de Planifium, des résultats académiques fournis par les enseignants ou les auxiliaires et des avis étudiants collectés via Discord, afin d’aider les étudiants à choisir leurs cours de manière éclairée.
L’application permet de rechercher, comparer et consulter des cours tout en personnalisant les recommandations selon le profil de l’étudiant.

## 🗂️ Organisation du répertoire

```text
Devoir1-2255/  
├─ docs/  
│  ├─ besoins/
│  │  ├─ diagrammes              → Dossier contenant les diagrammes flux + CUs 
│  │  ├─ cas-utilisation.md      → Cas d’utilisation et scénarios  
│  │  ├─ exigences.md            → Analyse des besoins   
│  │  ├─ flux-principaux.md      → Diagramme des flux d’informations  
│  │  ├─ glossaire.md            → Définitions des termes utilisés  
│  │  ├─ risques.md              → Analyse des risques  
│  ├─ conception/  
│  │  ├─ architecture.md         → Description de l’architecture globale  
│  │  ├─ C4_niveau1.png          → Modèle C4 – niveau 1  
│  │  └─ C4_niveau2.png          → Modèle C4 – niveau 2   
|  |
│  ├─ css/  
│  │  └─ no-sidebar.css          → Feuille de style personnalisée   
│  └─ index.md                   → Page d’accueil du site MkDocs  
│  
├─ mkdocs.yml                    → Fichier de configuration MkDocs  
├─ requirements.txt              → Dépendances Python  
├─ Pipfile                       → Environnement virtuel (pipenv)  
└─ README.md                     → Description du projet  
```


## Prototype interactif

Voici le lien permettant de visualiser le prototype interactif initial [Prototype](https://www.figma.com/make/oLDVLNKRifwxeUm5kLpRos/CourAdvisor--Copy-?node-id=0-1&p=f&t=6YJ55hxH3yMLNSCu-0&fullscreen=1).

Le prototype de CoursAdvisor comporte quatre pages principales. D’abord, la page d’accueil permet de se connecter ou de créer un compte étudiant à l’aide d’un courriel UdeM . Ensuite, la page du catalogue affiche la liste des cours avec leurs notes, difficultés et descriptions; l’utilisateur peut consulter les détails ou ajouter des cours à la comparaison. La page de comparaison permet d’analyser les cours à la fois selon leur charge de travail, difficulté et crédits .Enfin la page du profil permet d’ajuster les préférences pour personnaliser les recommandations.    

Note : Pour vous connecter, vous pouvez utiliser une adresse courriel au format suivant : aaaaa@aa.aa, ainsi que n’importe quel mot de passe.


## Prérequis

Assurez-vous d’avoir les outils suivants installés :

- Python **3.11** ou plus récent
- `pip` (gestionnaire de paquets Python)
- `pipenv` ou équivalent (gestion d’environnement virtuel) 
  - Évite de polluer votre système et les conflits de version.
  - Installez-le avec `pip install pipenv`.


## Installation

> Vous avez maintenant le contenu du template sur votre poste. Il ne reste qu’à installer les dépendances pour commencer à l’utiliser.

1. Activez l'environnement virtuel avec 
```bash
pipenv shell
```
2. Installez les dépendances listées dans `requirements.txt` (à exécuter dans le répertoire du projet) :

```bash
pip install -r requirements.txt
```

## Utilisation

> Avant toute utilisation, assurez-vous que l’environnement virtuel est activé (`pipenv shell`).

### Développement local

Pour lancer un serveur de développement local et visualiser les modifications en temps réel, utilisez :

```bash
mkdocs serve
```

Le site sera accessible à l'adresse [http://127.0.0.1:8000](http://127.0.0.1:8000)

### Construction du site (optionnel)

> Cette étape n’est pas nécessaire pour la publication sur GitHub Pages

Pour construire le site :

```bash
mkdocs build
```

Les fichiers générés seront dans le dossier `site/`.

### Déploiement

Pour déployer automatiquement le site sur GitHub Pages (branche `gh-pages`)

```bash
mkdocs gh-deploy
```

> Cette commande pousse automatiquement le contenu du site sur la branche `gh-pages`. Si la branche n'existe pas, elle est crée automatiquement.

## Structure du projet

- `docs/` : Contient tous les fichiers Markdown du site
- `mkdocs.yml` : Configuration de MkDocs
- `requirements.txt` : Dépendances Python
- `site/` : Site généré (créé lors de la construction) -- *optionnel*


## Licence

Ce projet est sous licence MIT. Voir le fichier `LICENSE` pour plus de détails.

## Ressources utiles

- Documentation officielle MkDocs
- Thème Material for MkDocs
>>>>>>> 70a4bd3c376cb037a051027718ee5c32014d421f
