# ss-mada — Page À propos

Page statique "À propos de nous" pour ss-mada, prête à être déployée sur **Cloudflare Pages** via GitHub.

---

## Structure du projet

```
ss-mada-about/
├── index.html      → La page complète
├── _headers        → En-têtes de sécurité Cloudflare
└── README.md       → Ce fichier
```

---

## Déploiement sur Cloudflare Pages via GitHub

### Étape 1 — Créer le dépôt GitHub

1. Allez sur [github.com](https://github.com) et connectez-vous
2. Cliquez sur **"New repository"**
3. Nommez-le par exemple `ss-mada-about`
4. Laissez-le en **Public** (nécessaire pour Cloudflare Pages gratuit)
5. Cliquez sur **"Create repository"**

### Étape 2 — Uploader les fichiers

Sur la page du dépôt vide :

1. Cliquez sur **"uploading an existing file"**
2. Glissez-déposez les 3 fichiers : `index.html`, `_headers`, `README.md`
3. Cliquez sur **"Commit changes"**

### Étape 3 — Connecter à Cloudflare Pages

1. Allez sur [pages.cloudflare.com](https://pages.cloudflare.com)
2. Connectez-vous ou créez un compte gratuit
3. Cliquez sur **"Create a project"** → **"Connect to Git"**
4. Autorisez Cloudflare à accéder à votre GitHub
5. Sélectionnez le dépôt `ss-mada-about`
6. Cliquez sur **"Begin setup"**

### Étape 4 — Configurer le build

Dans les paramètres de build, laissez tout **vide** (c'est un site statique, pas de build nécessaire) :

| Paramètre           | Valeur       |
|---------------------|--------------|
| Framework preset    | None         |
| Build command       | *(vide)*     |
| Build output dir    | *(vide)*     |

Cliquez sur **"Save and Deploy"**.

### Étape 5 — Votre site est en ligne

Cloudflare vous donnera une URL du type :
```
https://ss-mada-about.pages.dev
```

---

## Mettre à jour la page

À chaque modification de `index.html` sur GitHub, Cloudflare Pages redéploie automatiquement en quelques secondes.

---

## Domaine personnalisé (optionnel)

Si vous voulez utiliser `a-propos.ss-mada.com` :

1. Dans Cloudflare Pages → votre projet → **"Custom domains"**
2. Ajoutez votre domaine
3. Suivez les instructions DNS (si votre domaine est déjà sur Cloudflare, c'est automatique)

---

*Projet initié par Empire RK — Empire Groups, mai 2026.*
