# Live Incident — éditeur de visuels d'incident

Application web statique (un seul fichier `index.html`, JavaScript natif) qui génère une image 4K (ou Full HD)
à diffuser manuellement sur les écrans du personnel de conduite.

## Utilisation
1. **Créer un visuel** → choisir le modèle et la ligne.
2. Sélectionner les stations (mode « Tronçon » ou « Stations une à une »).
3. Saisir le titre et les informations.
4. Vérifier l'aperçu, puis **Télécharger l'image** (sur iPhone / iPad : « Enregistrer / Partager »).

Les brouillons et les visuels récents sont mémorisés **sur l'appareil** (stockage local du navigateur).

## Déploiement (GitHub Pages)
Settings → Pages → *Deploy from a branch* → `main` / `(root)`. Site : https://jrm-92.github.io/live_incident/

## Fichiers utilisés par le site
- `live_incident.png` (fond blanc, utilisé dans le visuel exporté), `live_incident_clair.png` (transparent, texte clair pour fonds sombres : accueil et barre du haut), `live_incident_transparent.png` (transparent, couleurs d'origine, pour fonds clairs), `logo_ligne9.png` : logos.
- `ralentissement_provisoire.png`, `service_securite.png`, `service_securite_sur_ordre.png`, `interruption_trafic.png`, `station_fermee.png` : images de consignes, chargées automatiquement.
- `Interstations/*.png` : schémas d'interstation de la ligne 9, chargés automatiquement. **Si un schéma est ajouté ou renommé, mettre à jour la liste `INTER_FILES` dans `index.html`.**
