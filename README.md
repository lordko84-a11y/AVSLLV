# Déploiement GitHub Pages — Vélo Saint‑Léger

Ce dossier est prêt pour **GitHub Pages** (site statique).

## Étapes rapides (utilisateur / organisation)
1) Créez un dépôt **public** nommé :
   - Utilisateur : `<votre-user>.github.io`
   - Organisation : `<votre-org>.github.io` ou un dépôt normal
2) Glissez ces fichiers à la racine du dépôt (`index.html`, `.nojekyll`, `robots.txt`, `sitemap.xml`).
3) Poussez sur `main` puis allez dans **Settings → Pages** :
   - **Source** : `Deploy from a branch`
   - **Branch** : `main` / `/ (root)`
4) Votre site sera accessible sur `https://<votre-user-ou-org>.github.io/`.

## Déploiement pour un dépôt projet (non `<user>.github.io`)
1) Dépôt public normal (ex: `asso-velo-site`).
2) **Settings → Pages** : Branche `main`, dossier `/ (root)`.
3) Activez Pages : l'URL sera `https://<votre-user>.github.io/asso-velo-site/`.
   - Si vous utilisez une URL de projet, vous pouvez ajouter une balise `<base href="/asso-velo-site/">` dans `<head>` si vous avez des assets relatifs (ici non nécessaire).

## Domaine personnalisé (optionnel)
- Renommez `CNAME.sample` en `CNAME` et remplacez par votre domaine (ex: `www.velosaintleger.fr`).
- Pointez votre domaine (DNS) vers GitHub Pages :
  - `A` → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
  - ou `CNAME` du sous-domaine → `<votre-user>.github.io`
- Dans **Settings → Pages → Custom domain**, entrez votre domaine puis **Save**.

## Modifier le contenu
- Le site est une **page unique** dans `index.html` (thème vert pastel).
- Pour une version React/Next.js, utilisez le composant dans `react/AssociationVeloSaintLeger.jsx` du pack précédent.

Bon déploiement 🚲
