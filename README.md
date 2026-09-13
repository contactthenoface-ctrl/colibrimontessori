# Mes Colibris Montessori — site web

## Structure
```
index.html      → la page du site
assets/         → logo + photos utilisées sur le site
```

## Mettre en ligne via GitHub (avec Termux)

1. Dézippe ce dossier, puis place-toi dedans dans Termux :
   ```bash
   cd mes-colibris-montessori
   ```

2. Initialise le dépôt Git et fais le premier commit :
   ```bash
   git init
   git add .
   git commit -m "Premier import du site Mes Colibris Montessori"
   ```

3. Crée un dépôt vide sur GitHub (sans README ni .gitignore), puis relie-le :
   ```bash
   git branch -M main
   git remote add origin https://github.com/<ton-compte>/<nom-du-repo>.git
   git push -u origin main
   ```

4. (Optionnel, pour publier gratuitement le site) Active **GitHub Pages** :
   Settings → Pages → Branch: `main` → dossier `/ (root)` → Save.
   Le site sera alors visible à l'adresse
   `https://<ton-compte>.github.io/<nom-du-repo>/`.

## À faire ensuite
- Remplacer `assets/galerie-3.jpg`, `galerie-4.jpg` et `galerie-5.jpg`
  (actuellement des photos génériques/illustration) par de vraies photos
  de l'école dès qu'elles seront disponibles, en gardant les mêmes noms
  de fichiers (ou en mettant à jour les balises `<img src="...">` dans
  `index.html`).
- Penser à réserver le nom de domaine `mescolibrismontessori.com` (ou
  équivalent) si ce n'est pas déjà fait, et à mettre à jour l'URL
  `canonical` et les balises Open Graph dans `index.html` en conséquence.
