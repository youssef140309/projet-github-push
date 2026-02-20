# GitHub Pédagogique

Support de cours progressif et participatif sur GitHub pour les élèves de Bac Pro CIEL, BTS CIEL et BTS SIO.

## 🎯 Objectif

Ce projet est un support de cours interactif qui permet aux élèves d'apprendre :
- Les bases de Git et GitHub
- Les commandes Git essentielles
- Comment pousser un projet sur GitHub
- Comment déployer un site sur Netlify

## 🚀 Installation

### Prérequis

- Node.js 18+ installé sur votre machine
- Git installé
- Un compte GitHub
- Un compte Netlify (gratuit)

### Installation locale

1. **Cloner le projet**
```bash
git clone https://github.com/votre-nom/github-pedagogique.git
cd github-pedagogique
```

2. **Installer les dépendances**
```bash
npm install
```

3. **Lancer le serveur de développement**
```bash
npm run dev
```

Le site sera accessible sur `http://localhost:4321`

## 📦 Déploiement sur Netlify

### Méthode 1 : Via l'interface Netlify (recommandée)

1. Créez un compte sur [netlify.com](https://www.netlify.com)
2. Connectez-vous avec votre compte GitHub
3. Cliquez sur "Add new site" → "Import an existing project"
4. Sélectionnez ce dépôt GitHub
5. Configurez le build :
   - **Build command** : `npm run build`
   - **Publish directory** : `dist`
6. Cliquez sur "Deploy site"

### Méthode 2 : Via la ligne de commande

```bash
# Installer Netlify CLI
npm install -g netlify-cli

# Se connecter à Netlify
netlify login

# Déployer
netlify deploy --prod
```

## 📚 Structure du projet

```
github-pedagogique/
├── src/
│   ├── layouts/
│   │   └── Layout.astro          # Layout principal
│   ├── pages/
│   │   ├── index.astro           # Page d'accueil
│   │   ├── cours.astro           # Page de cours
│   │   └── qcm.astro             # QCM final
│   └── styles/
│       └── global.css            # Styles globaux
├── public/
│   └── images/                   # Images du site
├── astro.config.mjs              # Configuration Astro
├── tailwind.config.mjs           # Configuration Tailwind
├── package.json                  # Dépendances
└── README.md                     # Ce fichier
```

## ✨ Fonctionnalités

- ✅ Cours progressif sur GitHub
- ✅ Exercices pratiques intégrés
- ✅ QCM de 20 questions
- ✅ Sauvegarde automatique des réponses (localStorage)
- ✅ Possibilité de reprendre où on s'est arrêté
- ✅ Envoi des résultats par email
- ✅ Design responsive
- ✅ Déploiement automatique sur Netlify

## 🎓 Utilisation pédagogique

Ce support de cours est conçu pour :
1. Être suivi de manière autonome par les élèves
2. Permettre aux élèves de pratiquer sur le projet lui-même
3. Valider les connaissances via le QCM final

Les élèves peuvent envoyer leurs résultats du QCM à leur enseignant à l'adresse : **mormin@st-nicolas.fr**

## 🛠️ Technologies utilisées

- [Astro](https://astro.build) - Framework web moderne
- [Tailwind CSS](https://tailwindcss.com) - Framework CSS
- [Netlify](https://netlify.com) - Hébergement et déploiement

## 📝 Licence

© 2026 Eric MORMIN — Tous droits réservés

Édité par [EKM Conseils](https://www.ekmconseils.eu)

Ressource pédagogique réalisée pour La Salle Saint-Nicolas, Issy-les-Moulineaux

Bac Pro CIEL, BTS CIEL, BTS SIO

## 👨‍🏫 Auteur

**Eric MORMIN**  
Email : mormin@st-nicolas.fr  
Site : [www.ekmconseils.eu](https://www.ekmconseils.eu)

---

Version 1.0.0
