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
- `banque/*.png` : banque d'images (rame, signaux, indicateurs SP, plaques…) à ajouter au visuel à l'étape 3. Pour ajouter une image, la déposer dans ce dossier et l'ajouter à la liste `BANK` dans `index.html`.
- Images de consignes et schémas d'interstation : retirés. Chaque utilisateur importe ses propres images (QR code, schéma…) à l'étape 3, dans « Images et QR codes ».
