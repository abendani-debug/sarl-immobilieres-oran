# Guide de Déploiement sur Vercel - SARL Immobilières Algérienne

## 📋 Fichiers Prêts pour le Déploiement

Vous avez les fichiers suivants dans le dossier `/mnt/user-data/outputs/`:
- ✅ `index.html` - Site vitrine complet
- ✅ `logo.png` - Logo de votre entreprise
- ✅ `vercel.json` - Configuration Vercel

## 🚀 Méthode 1 : Déploiement via GitHub (Recommandé)

### Étape 1 : Créer un repository GitHub
1. Allez sur https://github.com/new
2. Créez un nouveau repository appelé `sarl-immobilieres-oran`
3. Ne cochez PAS "Initialize this repository with a README"

### Étape 2 : Pousser les fichiers vers GitHub
```bash
cd /chemin/vers/votre/dossier
git remote add origin https://github.com/VOTRE_USERNAME/sarl-immobilieres-oran.git
git branch -M main
git push -u origin main
```

### Étape 3 : Connecter à Vercel
1. Allez sur https://vercel.com
2. Connectez-vous ou créez un compte gratuit
3. Cliquez sur "Add New..." → "Project"
4. Sélectionnez votre repository GitHub
5. Vercel détectera automatiquement la configuration
6. Cliquez sur "Deploy"

**Votre site sera en ligne en quelques secondes !** 🎉

---

## 🚀 Méthode 2 : Déploiement Direct via CLI Vercel

### Étape 1 : Installer Vercel CLI
```bash
npm install -g vercel
```

### Étape 2 : Déployer depuis le dossier du projet
```bash
cd /chemin/vers/votre/dossier
vercel
```

### Étape 3 : Suivre les instructions
- Acceptez les paramètres par défaut
- Authentifiez-vous avec votre compte Vercel
- Vercel fera le déploiement automatiquement

---

## 🚀 Méthode 3 : Import Direct depuis un Fichier ZIP

1. Créez un ZIP de votre dossier contenant:
   - index.html
   - logo.png
   - vercel.json

2. Allez sur https://vercel.com/import
3. Uploadez votre fichier ZIP
4. Suivez les instructions de déploiement

---

## ✨ Après le Déploiement

Une fois déployé, vous recevrez une URL comme:
```
https://sarl-immobilieres-oran.vercel.app
```

### Ajouter un Domaine Personnalisé
1. Dans le dashboard Vercel
2. Allez dans "Settings" → "Domains"
3. Ajoutez votre domaine (ex: www.sarl-immobilieres-oran.dz)
4. Configurez les DNS records selon les instructions

---

## 📞 Support et Configuration

### Pour mettre à jour le site:
- Modifiez les fichiers localement
- Faites un `git push` vers GitHub
- Vercel redéploiera automatiquement !

### Variables d'Environnement (si nécessaire):
Créez un fichier `.env.local`:
```
NEXT_PUBLIC_API_URL=votre_url_api
```

### Fichiers Importants:
- **vercel.json** : Configuration du projet
- **index.html** : Page principale
- **.gitignore** : Fichiers à ignorer (optionnel)

---

## 🎯 Checklist Finale

- [ ] Repository GitHub créé
- [ ] Fichiers pushés vers GitHub
- [ ] Compte Vercel créé
- [ ] Projet importé dans Vercel
- [ ] URL de déploiement testée
- [ ] Domaine personnalisé configuré (optionnel)

---

## 💡 Conseils

✅ **Gratuit** : Vercel offre un plan gratuit parfait pour les sites statiques
✅ **Performant** : CDN global pour une livraison ultra-rapide
✅ **Sécurisé** : HTTPS automatique sur tous les sites
✅ **Facile** : Déploiement automatique à chaque push Git

---

**Besoin d'aide ?** 
- Documentation Vercel: https://vercel.com/docs
- Support: https://vercel.com/support
