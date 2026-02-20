# 🚀 Installation rapide - GitHub Pédagogique

## Démarrage rapide (5 minutes)

### 1. Télécharger le projet
Vous avez déjà le projet, parfait !

### 2. Installer Node.js
Si vous n'avez pas Node.js :
- Téléchargez depuis [nodejs.org](https://nodejs.org)
- Installez la version LTS (recommandée)
- Vérifiez : `node --version`

### 3. Installer les dépendances
```bash
cd github-pedagogique
npm install
```

### 4. Lancer le site en local
```bash
npm run dev
```

Le site sera accessible sur : **http://localhost:4321**

---

## 📚 Prochaines étapes

1. **Suivre le cours** : Ouvrez http://localhost:4321 et suivez les leçons
2. **Pousser sur GitHub** : Consultez `GUIDE_DEPLOIEMENT.md` pour les instructions détaillées
3. **Déployer sur Netlify** : Suivez le guide de déploiement

---

## 📁 Structure du projet

```
github-pedagogique/
├── src/
│   ├── pages/
│   │   ├── index.astro    # Page d'accueil
│   │   ├── cours.astro    # Cours complet
│   │   └── qcm.astro      # QCM de 20 questions
│   ├── layouts/
│   │   └── Layout.astro   # Layout principal
│   └── styles/
│       └── global.css     # Styles globaux
├── public/                # Fichiers statiques
├── README.md              # Documentation
├── GUIDE_DEPLOIEMENT.md   # Guide complet pour GitHub + Netlify
└── package.json           # Dépendances du projet
```

---

## ⚡ Commandes utiles

```bash
npm run dev        # Démarre le serveur de développement
npm run build      # Crée la version de production
npm run preview    # Prévisualise la version de production
```

---

## 🆘 Besoin d'aide ?

- Consultez le `GUIDE_DEPLOIEMENT.md` pour les instructions complètes
- Lisez le `README.md` pour plus de détails
- Contactez votre enseignant : mormin@st-nicolas.fr

---

**Bon cours ! 📖**
