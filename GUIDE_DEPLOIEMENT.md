# 📘 Guide de déploiement - GitHub Pédagogique

Ce guide vous accompagne pas à pas pour pousser ce projet sur GitHub et le déployer sur Netlify.

## 🎯 Objectif

À la fin de ce guide, vous aurez :
1. ✅ Poussé ce projet sur VOTRE compte GitHub
2. ✅ Déployé le site en ligne sur Netlify
3. ✅ Un site accessible publiquement avec une URL

---

## Étape 1 : Installer Git

### Windows
1. Téléchargez Git depuis [git-scm.com](https://git-scm.com/download/win)
2. Lancez l'installateur et suivez les étapes (gardez les options par défaut)
3. Vérifiez l'installation :
   ```bash
   git --version
   ```

### macOS
```bash
brew install git
```

### Linux (Ubuntu/Debian)
```bash
sudo apt-get install git
```

---

## Étape 2 : Configurer Git

Configurez votre identité (remplacez par vos informations) :

```bash
git config --global user.name "Votre Nom"
git config --global user.email "votre.email@example.com"
```

Vérifiez la configuration :
```bash
git config --list
```

---

## Étape 3 : Créer un compte GitHub

1. Allez sur [github.com](https://github.com)
2. Cliquez sur "Sign up"
3. Remplissez le formulaire avec :
   - Un nom d'utilisateur unique
   - Votre email
   - Un mot de passe sécurisé
4. Vérifiez votre email
5. Complétez votre profil (optionnel mais recommandé)

---

## Étape 4 : Créer un nouveau dépôt sur GitHub

1. Connectez-vous à GitHub
2. Cliquez sur le bouton **"+"** en haut à droite
3. Sélectionnez **"New repository"**
4. Remplissez les informations :
   - **Repository name** : `github-pedagogique` (ou un autre nom)
   - **Description** : "Support de cours sur GitHub"
   - **Public** ou **Private** : Choisissez Public pour partager
   - ⚠️ **NE cochez PAS** "Add a README file"
   - ⚠️ **NE cochez PAS** "Add .gitignore"
5. Cliquez sur **"Create repository"**

GitHub va vous afficher une page avec des instructions. **Gardez cette page ouverte**, vous en aurez besoin !

---

## Étape 5 : Initialiser le projet localement

Ouvrez votre terminal (PowerShell sur Windows, Terminal sur Mac/Linux) et naviguez vers le dossier du projet :

```bash
cd chemin/vers/github-pedagogique
```

Initialisez Git dans ce dossier :
```bash
git init
```

Vous devriez voir le message : `Initialized empty Git repository in ...`

---

## Étape 6 : Ajouter tous les fichiers

Ajoutez tous les fichiers du projet au suivi Git :

```bash
git add .
```

> **Note** : Le point `.` signifie "tous les fichiers"

Vérifiez que les fichiers sont bien ajoutés :
```bash
git status
```

Vous devriez voir tous vos fichiers en vert.

---

## Étape 7 : Créer votre premier commit

Créez un commit avec un message descriptif :

```bash
git commit -m "Premier commit - Ajout du projet GitHub Pédagogique"
```

---

## Étape 8 : Lier votre dépôt local à GitHub

Retournez sur la page GitHub que vous avez gardée ouverte à l'Étape 4.

Copiez l'URL de votre dépôt (elle ressemble à : `https://github.com/votre-nom/github-pedagogique.git`)

Dans votre terminal, tapez :

```bash
git remote add origin https://github.com/VOTRE-NOM/github-pedagogique.git
```

> ⚠️ **Remplacez** `VOTRE-NOM` par votre vrai nom d'utilisateur GitHub !

Vérifiez la connexion :
```bash
git remote -v
```

Vous devriez voir deux lignes avec l'URL de votre dépôt.

---

## Étape 9 : Changer le nom de la branche (si nécessaire)

Par défaut, Git crée une branche "master", mais GitHub utilise "main". Renommez-la :

```bash
git branch -M main
```

---

## Étape 10 : Pousser votre code sur GitHub

Envoyez votre code sur GitHub :

```bash
git push -u origin main
```

> **Note** : L'option `-u` permet de définir la branche par défaut. Vous n'aurez plus besoin de l'utiliser par la suite.

Si c'est votre première fois, Git vous demandera peut-être de vous authentifier avec GitHub.

---

## Étape 11 : Vérifier sur GitHub

1. Retournez sur GitHub
2. Rafraîchissez la page de votre dépôt
3. Vous devriez voir tous vos fichiers ! 🎉

---

## 🚀 PARTIE 2 : Déploiement sur Netlify

Maintenant que votre projet est sur GitHub, on va le déployer en ligne !

---

## Étape 12 : Créer un compte Netlify

1. Allez sur [netlify.com](https://www.netlify.com)
2. Cliquez sur **"Sign up"**
3. Choisissez **"Sign up with GitHub"**
4. Autorisez Netlify à accéder à votre compte GitHub
5. Confirmez votre email si demandé

---

## Étape 13 : Connecter votre dépôt GitHub

1. Une fois connecté, cliquez sur **"Add new site"**
2. Sélectionnez **"Import an existing project"**
3. Cliquez sur **"Deploy with GitHub"**
4. Autorisez Netlify à accéder à vos dépôts (si demandé)
5. Cherchez et sélectionnez votre dépôt `github-pedagogique`

---

## Étape 14 : Configurer le build

Netlify détecte automatiquement qu'il s'agit d'un projet Astro. Vérifiez les paramètres :

- **Branch to deploy** : `main`
- **Build command** : `npm run build`
- **Publish directory** : `dist`

> Si ces champs ne sont pas remplis, ajoutez-les manuellement.

Cliquez sur **"Deploy site"**

---

## Étape 15 : Attendre le déploiement

Netlify va :
1. Installer les dépendances (`npm install`)
2. Construire le projet (`npm run build`)
3. Déployer le site

Cela prend généralement 1-2 minutes. Vous verrez les logs en temps réel.

---

## Étape 16 : Accéder à votre site

Une fois le déploiement terminé :

1. Netlify vous donne une URL aléatoire comme : `random-name-123456.netlify.app`
2. Cliquez sur l'URL pour voir votre site en ligne ! 🎉

---

## Étape 17 : Personnaliser le nom de domaine

1. Dans Netlify, allez dans **"Site settings"**
2. Cliquez sur **"Change site name"**
3. Entrez un nom personnalisé (ex: `mon-cours-github`)
4. Votre nouvelle URL sera : `mon-cours-github.netlify.app`

---

## ✨ Mises à jour automatiques

Le plus magique : chaque fois que vous faites un `git push`, Netlify redéploie automatiquement votre site !

**Workflow pour les mises à jour :**

```bash
# 1. Modifier vos fichiers localement
# 2. Ajouter les modifications
git add .

# 3. Créer un commit
git commit -m "Description de vos modifications"

# 4. Pousser sur GitHub
git push

# 5. Netlify redéploie automatiquement ! 🚀
```

---

## 🎓 Félicitations !

Vous avez maintenant :
- ✅ Un dépôt GitHub avec votre code
- ✅ Un site web déployé et accessible en ligne
- ✅ Un workflow de déploiement continu

**Notez votre URL Netlify et partagez-la avec votre enseignant !**

---

## 🆘 Problèmes courants

### Erreur "permission denied" lors du push
- Vérifiez que vous êtes bien authentifié sur GitHub
- Utilisez `git remote -v` pour vérifier l'URL du dépôt

### Le build échoue sur Netlify
- Vérifiez que vous avez bien un fichier `package.json`
- Vérifiez que la commande de build est `npm run build`
- Consultez les logs d'erreur dans Netlify

### Le site ne s'affiche pas correctement
- Vérifiez que le "Publish directory" est bien `dist`
- Attendez quelques minutes que le déploiement se propage

---

## 📧 Support

Pour toute question, contactez votre enseignant :  
**mormin@st-nicolas.fr**

---

**Bon courage et bonne chance ! 🚀**
