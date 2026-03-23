# MineLab Pro — Déploiement Vercel

Application de gestion de laboratoire minier développée par **HabaTech**.

## 📁 Structure du projet

```
minelab-pro/
├── index.html      ← Application principale (single-file)
├── vercel.json     ← Configuration Vercel
└── README.md       ← Ce fichier
```

## 🚀 Déploiement sur Vercel

### Méthode 1 — Via GitHub (Recommandé)

1. Crée un nouveau repo GitHub (ex: `minelab-pro`)
2. Upload les fichiers `index.html` et `vercel.json`
3. Va sur [vercel.com](https://vercel.com) → **New Project**
4. Importe ton repo GitHub
5. Clique **Deploy** → C'est tout ! ✅

Ton site sera live sur : `minelab-pro.vercel.app`

### Méthode 2 — Via Vercel CLI

```bash
npm install -g vercel
vercel login
vercel --prod
```

### Méthode 3 — Drag & Drop

1. Va sur [vercel.com/new](https://vercel.com/new)
2. Glisse-dépose le dossier du projet
3. Déploiement automatique ✅

## ⚙️ Configuration Supabase

Assure-toi que ton projet Supabase a les bonnes **URL autorisées** :

1. Va dans **Supabase Dashboard** → Authentication → URL Configuration
2. Ajoute dans **Site URL** : `https://minelab-pro.vercel.app`
3. Ajoute dans **Redirect URLs** : `https://minelab-pro.vercel.app/**`

## 🔄 Mises à jour

Chaque `git push` sur GitHub déclenche un **redéploiement automatique** — sans limites de build minutes !

---

Développé par **HabaTech** — Solutions numériques · Conakry, Guinée  
WhatsApp : +224 627 541 925
