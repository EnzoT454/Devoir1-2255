# Template de site web pour IFT2255

Ce projet est un template pour le rapport à produire pour le cours IFT2255 (Génie logiciel), construit avec [MkDocs](https://www.mkdocs.org/) et le thème [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).

## CoursAdvisor (Brève description)
 
**CoursAdviso** est une plateforme web destinée aux étudiants du DIRO (Université de Montréal).
Elle centralise les données provenant de Planifium, des résultats académiques et des avis étudiants collectés via Discord, afin d’aider les étudiants à choisir leurs cours de manière éclairée.
L’application permet de rechercher, comparer et consulter des cours tout en personnalisant les recommandations selon le profil de l’étudiant.

## 🗂️ Organisation du répertoire


Devoir1-2255/  
├─ docs/  
│  ├─ besoins/  
│  │  ├─ cas-utilisation.md      → Cas d’utilisation et scénarios  
│  │  ├─ exigences.md            → Analyse des besoins   
│  │  ├─ flux-principaux.md      → Diagramme des flux d’informations  
│  │  ├─ glossaire.md            → Définitions des termes utilisés  
│  │  ├─ risques.md              → Analyse des risques  
│  ├─ conception/  
│  │  ├─ architecture.md         → Description de l’architecture globale  
│  │  ├─ C4_niveau1.png          → Modèle C4 – niveau 1  
│  │  ├─ C4_niveau2.png          → Modèle C4 – niveau 2   
│  │  ├─ uml.md                  → Diagrammes UML  
│  │  └─ modeles.md              → Schémas et modèles de données  
│  ├─ css/  
│  │  └─ no-sidebar.css          → Feuille de style personnalisée  
│  ├─ application.md             → Documentation sur l’application  
│  ├─ evaluation.md              → Évaluation du projet  
│  ├─ bilan.md                   → Bilan final  
│  └─ index.md                   → Page d’accueil du site MkDocs  
│  
├─ mkdocs.yml                    → Fichier de configuration MkDocs  
├─ requirements.txt              → Dépendances Python  
├─ Pipfile                       → Environnement virtuel (pipenv)  
└─ README.md                     → Description du projet   

## Prérequis

Assurez-vous d’avoir les outils suivants installés :

- Python **3.11** ou plus récent
- `pip` (gestionnaire de paquets Python)
- `pipenv` ou équivalent (gestion d’environnement virtuel) 
  - Évite de polluer votre système et les conflits de version.
  - Installez-le avec `pip install pipenv`.

## Pour commencer

### Option 1: Le répertoire n'est pas encore créé

1. Cliquez sur le bouton `Use this template` sur GitHub.
2. Choisissez l'option `Create a new repository`.
3. À la fin des étapes, vous devriez avoir un nouveau répertoire avec le contenu du template.

### Option 2: Le répertoire existe déjà

1. Clonez ce dépôt (optionnel) pour obtenir le template localement 
```bash
git clone git@github.com:udem-diro/template-rapport-ift2255.git
```
2. Copiez les fichiers du template (en local) dans votre répertoire de projet.

> Note : Cette option est utile si vous souhaitez récupérer le contenu du template sans créer un nouveau dépôt (répertoire).

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

## Personnalisation

1. Modifiez `mkdocs.yml` pour changer la configuration du site
2. Ajoutez/modifiez les fichiers Markdown (`.md`) dans `docs/`
3. Personnalisez le thème en modifiant les paramètres dans `mkdocs.yml`

## Licence

Ce projet est sous licence MIT. Voir le fichier `LICENSE` pour plus de détails.

## Ressources utiles

- Documentation officielle MkDocs
- Thème Material for MkDocs