# Check-up Matinal 🌿

App de check-up digestif quotidien — Le Garde du Corps Digestif (Gemini AI).

## Fichiers

```
index.html    → App complète (HTML/CSS/JS, single-file)
vercel.json   → Config de routing Vercel
```

## Déploiement GitHub + Vercel

### 1. Créer le repo GitHub

```bash
# Dans ton terminal, depuis le dossier du projet
git init
git add .
git commit -m "feat: check-up matinal initial"
git branch -M main
git remote add origin https://github.com/TON_USERNAME/checkup-matinal.git
git push -u origin main
```

### 2. Connecter à Vercel

1. Va sur [vercel.com](https://vercel.com) → **Add New Project**
2. Importe ton repo GitHub `checkup-matinal`
3. Framework Preset → **Other**
4. Root Directory → laisser `.`
5. Clique **Deploy**

→ Vercel te donne une URL du type `checkup-matinal.vercel.app`

### 3. Accès mobile

Ajoute l'URL en raccourci sur ton écran d'accueil iPhone :
- Safari → ouvrir l'URL → icône Partager → **"Sur l'écran d'accueil"**

## Notes

- **API key** : la clé Gemini est intégrée dans `index.html`. Pour la sécuriser davantage, tu peux passer par une Vercel Edge Function qui fait proxy, mais pour usage personnel c'est suffisant.
- **Stack** : Vanilla HTML/CSS/JS, zéro dépendance, zéro build step.
