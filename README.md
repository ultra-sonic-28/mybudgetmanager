# MyBudgetManager (MBM)

Logiciel open source qui vous aide maîtriser vos comptes, anticiper vos dépenses et garder le contrôle de votre budget.

## Description

**MyBudgetManager (MBM)** est une application de gestion budgétaire personnelle permettant de centraliser et de suivre l'ensemble de ses finances au quotidien. Elle offre la gestion de plusieurs comptes, des recettes et dépenses, des transferts et avances, ainsi que le suivi des opérations récurrentes et des projets prévisionnels. Grâce à ses tableaux de bord, statistiques et outils de rapprochement bancaire, elle permet de visualiser l'évolution de ses finances, de maîtriser son budget et d'anticiper sa trésorerie. Développée pour Windows, elle privilégie la simplicité d'utilisation, la personnalisation et le stockage local des données.

## Mentions Légales

**MyBudgetManager** est un outil indépendant, gratuit, à but non lucratif et en open source, conçu pour faciliter la gestion de votre argent.

Cette application n’est **ni affiliée à, ni approuvée par, ni sponsorisée par** un quelconque établissement bancaire.

Toutes les marques mentionnées (le cas échéant) sont la propriété de leurs détenteurs respectifs.

Tous les éléments visuels ont été soit créés spécifiquement pour ce projet, soit distribués sous licence CC0 (domaine public) ou sous des licences libres compatibles.

## Fonctionnalités

### 1. Gestion des comptes

- Création et gestion de plusieurs comptes : courants, épargne, espèces et autres.
- Paramétrage des soldes initiaux et des dates d'ouverture.
- Consultation des soldes par compte et du solde global.
- Activation, désactivation et clôture des comptes.

### 2. Gestion des opérations

- Saisie des recettes et des dépenses.
- Gestion des dates, libellés, tiers, catégories et types de paiement.
- Suivi des numéros de chèques.
- Pointage des opérations.
- Ventilation d'une opération sur plusieurs catégories ou sous-catégories.
- Recherche, filtrage, modification et duplication des opérations.
- Calcul automatique des soldes comptables et bancaires.

### 3. Transferts et avances

- Transferts entre les différents comptes.
- Suivi des mouvements associés à chaque transfert.
- Gestion des frais éventuels liés aux transferts.
- Enregistrement des avances accordées à des tiers.
- Suivi des remboursements partiels ou complets.
- Consultation des montants restant à récupérer.

### 4. Gestion des catégories et des tiers

- Création et personnalisation des catégories et sous-catégories.
- Classement des recettes et des dépenses.
- Gestion des tiers : particuliers, entreprises, organismes, fournisseurs, etc.
- Conservation de l'historique des catégories et tiers utilisés.

### 5. Gestion des opérations récurrentes

- Création de règles de mensualisation.
- Gestion des recettes et dépenses périodiques.
- Définition de montants variables selon les mois.
- Génération automatique des échéances.
- Transformation des échéances en opérations réelles.
- Modification ou annulation d'une échéance.

### 6. Gestion des dépenses prévisionnelles et des projets

- Création de projets avec budget et dates prévisionnelles.
- Définition de plusieurs échéances par projet.
- Planification des dépenses sur plusieurs mois.
- Gestion des paiements partiels ou multiples.
- Suivi des budgets consommés et des montants restant à payer.
- Intégration des échéances dans les prévisions de trésorerie.

### 7. Rapprochement bancaire

- Création de rapprochements à partir des relevés bancaires.
- Sélection des opérations correspondantes.
- Calcul automatique des soldes et des écarts.
- Validation des rapprochements.
- Conservation de l'historique des rapprochements.
- Protection des opérations déjà rapprochées.

### 8. Tableaux de bord et statistiques

- Synthèse annuelle et mensuelle des recettes et dépenses.
- Visualisation de l'évolution des soldes.
- Suivi des soldes comptables et bancaires.
- Graphiques des recettes et dépenses par mois.
- Répartition des dépenses par catégories et sous-catégories.
- Analyse des dépenses par tiers.
- Comparaison des différents comptes.
- Suivi des avances et des projets.
- Prévisions de trésorerie.

### 9. Recherche et exploitation des données

- Recherche multicritère des opérations.
- Filtres par période, compte, catégorie, tiers et type d'opération.
- Tri des résultats selon différents critères.
- Export des données au format CSV et Excel.

### 10. Importation et migration des données

- Importation des données depuis le classeur Excel existant.
- Récupération des catégories, tiers et opérations historiques.
- Importation des mensualisations et dépenses prévisionnelles.
- Contrôle des données importées et détection des anomalies.
- Rapport détaillé des éventuelles erreurs d'importation.

## 11. Administration et sécurité des données

- Stockage local des données dans une base SQLite.
- Sauvegardes manuelles et automatiques.
- Restauration des sauvegardes.
- Historisation des événements importants.
- Contrôle de l'intégrité des données.

## Installation

### Prérequis

- Python 3.13 ou version ultérieure
- Windows 10/11

### Installation à partir des sources

Ouvrez un terminal et exécutez les commandes suivantes :

    # Cloner le dépôt
    git clone https://github.com/ultra-sonic-28/mybudgetmanager.git
    cd mybudgetmanager

    # Commencez à coder
    # en utilisant votre éditeur de code préféré

## Développement

### Structure du projet

    mybudgetmanager/
    ├── src/mybudgetmanager/                     # Sources Python (paquet importable)
    │   ├── main.py                              # Point d’entrée principal pour MyBudgetManager
    │   ├── utils/                               # Utilitaires partagés
    │   └── ui/                                  # Interface utilisateur
    │       ├── dialogs/                         # Fenêtres de dialogue
    │       ├── widgets/                         # Composants réutilisables
    │       └── windows/                         # Fenêtres
    ├── mybudgetmanager.code-workspace           # Fichier d’espace de travail VS Code
    ├── README.md                                # README principal avec avertissement
    ├── LICENSE                                  # Licence MIT
    ├── .gitignore                               # .gitignore
    ├── .vscode/                                 # Paramètres de l’espace de travail Visual Studio Code
    ├── assets/                                  # Ressources partagées (CC0 uniquement)
    └── tests/                                   # Dossiers de tests
        ├── integration/                         # Tests d’intégration
        ├── unit/                                # Tests unitaires
        ├── ui/                                  # Tests d’interface utilisateur
        └── utils/                               # Tests des classes / fonctions utilitaires

## Licence

Ce projet est sous licence MIT. Consultez le fichier [LICENSE](LICENSE) pour plus de détails.

---

**Dernière mise à jour**: 2026-11-16
