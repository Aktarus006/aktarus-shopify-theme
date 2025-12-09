# Aktarus Shopify Theme - Projet de Formation

[![Generic badge](https://img.shields.io/badge/course%20available%3F-yes-green.svg)](https://shields.io/)

Projet de développement de thème Shopify basé sur le cours [Shopify Theme Development – Online Store 2.0 + TailwindCSS](https://weeklyhow.com/courses/)

## 🚀 Installation & Setup

### Prérequis

- [Node.js](https://nodejs.org/) (v18+)
- [Shopify CLI](https://shopify.dev/themes/tools/cli/installation)
- Git

### Installation

1. **Cloner le projet**

   ```bash
   git clone <your-repo-url>
   cd aktarus-theme-tuto
   ```

2. **Installer les dépendances**

   ```bash
   npm install
   ```

3. **Connexion à Shopify**

   ```bash
   shopify auth login
   ```

4. **Lancer le développement**

   Dans deux terminaux séparés:

   **Terminal 1 - Tailwind CSS:**

   ```bash
   npx tailwindcss -i ./src/tailwind.css -o ./assets/application.css --watch
   ```

   **Terminal 2 - Shopify Dev Server:**

   ```bash
   shopify theme dev
   ```

   Ouvrir `http://127.0.0.1:9292` dans votre navigateur

## 📦 Scripts Disponibles

```bash
npm run format         # Formater tous les fichiers avec Prettier
npm run format:check   # Vérifier le formatage sans modifier
npm run theme:check    # Vérifier les erreurs Shopify Theme
```

## 🛠️ Stack Technique

- **Shopify Liquid** - Langage de template
- **Tailwind CSS 4** - Framework CSS utilitaire
- **Prettier** - Formatage automatique du code
- **Husky** - Git hooks (pre-commit)
- **Theme Check** - Linter pour thèmes Shopify

## 🔧 Extensions VS Code Recommandées

Le projet inclut un fichier `.vscode/extensions.json` qui recommande automatiquement les extensions essentielles:

- **Shopify Theme Check** - Linter pour thèmes Shopify
- **Prettier** - Formatage automatique du code
- **Tailwind CSS IntelliSense** - Autocomplétion Tailwind
- **GitLens** - Historique Git avancé
- **Error Lens** - Affichage inline des erreurs
- **Code Spell Checker** (EN + FR) - Vérification orthographique
- **Auto Rename Tag** - Renommage automatique des balises
- **Live Share** - Collaboration en temps réel
- **TODO Tree** - Gestion des TODO/FIXME dans le code
- **Bookmarks** - Navigation rapide dans le code

### TODO Tree

Utilisez ces tags dans vos commentaires pour organiser les tâches:

```liquid
{% comment %}
  TODO: Implémenter la fonctionnalité X
  FIXME: Corriger le bug de prix
  HACK: Code temporaire à refactoriser
  NOTE: Information importante
  BUG: Bug connu à résoudre
{% endcomment %}
```

Tous les TODOs apparaissent dans la barre latérale pour un suivi facile.

## 📝 Conventions de Code

### Branches Git

- `main` - Branche principale (production)
- `feature/*` - Nouvelles fonctionnalités
- `fix/*` - Corrections de bugs
- `hotfix/*` - Corrections urgentes

### Commits

Le projet utilise **Husky** pour formater automatiquement le code avant chaque commit.

Les fichiers suivants sont formatés automatiquement:

- `*.liquid` - Fichiers Liquid
- `*.json` - Fichiers de configuration
- `*.js` - JavaScript
- `*.css` - CSS

### Structure des Fichiers

```
.
├── assets/          # CSS, JS, images compilés
├── blocks/          # Composants réutilisables
├── config/          # Configuration du thème
├── layout/          # Layout principal
├── locales/         # Traductions
├── sections/        # Sections du thème
├── snippets/        # Snippets réutilisables
├── src/             # Sources Tailwind
└── templates/       # Templates de pages
```

## 🎓 Leçons Couvertes

| Status | Leçon                                    |
| ------ | ---------------------------------------- |
| ✅     | Installation des outils de développement |
| ✅     | Barre de navigation                      |
| ✅     | Page 404                                 |
| ✅     | Page Article                             |
| ✅     | Page Blog                                |
| ✅     | Panier                                   |
| ✅     | Page Collection                          |
| ✅     | Page Collections                         |
| ✅     | Page d'accueil                           |
| ✅     | Pages (À propos & Contact)               |
| ✅     | Page Produit avancée                     |
| ✅     | Page Recherche                           |
| 🔄     | Plus de leçons à venir                   |

## 🤝 Collaboration

Ce projet est configuré pour le travail en équipe avec:

- Formatage automatique du code (Prettier + Husky)
- Extensions VS Code partagées
- Configuration SSH pour authentification
- Git hooks pour maintenir la qualité du code

## 📚 Ressources

- [Documentation Shopify Liquid](https://shopify.dev/docs/api/liquid)
- [Documentation Tailwind CSS](https://tailwindcss.com/docs)
- [Shopify CLI Documentation](https://shopify.dev/themes/tools/cli)

## 📄 Licence

Ce projet est un projet de formation basé sur le cours Udemy de WeeklyHow.
