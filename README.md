# IBQ DJ

Site React responsive basé sur la maquette 1.

## Démarrer
npm install
npm run dev -- --host 127.0.0.1 --port 4173

## Production
npm run build
npm run test:sites

Le résultat statique est dans dist/client. Le projet conserve aussi le Worker et les métadonnées du modèle Product Design pour une future publication Sites.

## Modifier
src/App.jsx : contenus, liens et vidéos.
src/styles.css : présentation et mobile.
public/assets : visuels.

Les boutons Spotify ouvrent l'album original. Les clips utilisent YouTube. Le contact ouvre la messagerie locale. Aucun message n'est envoyé automatiquement.

## GitHub Pages
Ce dossier doit être placé à la racine du dépôt GitHub dédié à IBQ DJ.
Dans Settings > Pages > Build and deployment, choisir GitHub Actions.
Le workflow .github/workflows/deploy-pages.yml construit et déploie dist/client à chaque push sur main. Les chemins relatifs permettent une publication sous /ibq-dj/ sans perdre les images.
