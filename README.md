# Planning Atelier AMS

Planning hebdomadaire de l'atelier : les commerciaux déposent les BL (PDF) et les placent sur la semaine,
l'atelier consulte le planning, coche « Terminé » et envoie des notes aux commerciaux.
Tout est synchronisé en direct entre tous les appareils.

- Accès commercial : bouton « Accès commercial », code **4567**.
- Vue atelier : par défaut, pour tout le monde.

## Mise en route (une seule fois, ~5 min)

1. Aller sur https://console.firebase.google.com avec un compte Google AMS → **Ajouter un projet** (nom : `ams-planning`, Google Analytics inutile).
2. Menu **Créer → Firestore Database** → **Créer une base de données** → emplacement `eur3 (europe-west)` → mode **production**.
3. Onglet **Règles** : coller le contenu du fichier `firestore.rules` → **Publier**.
4. Roue crantée **Paramètres du projet** → **Vos applications** → icône **Web `</>`** → nom `planning` → **Enregistrer**.
   Copier les valeurs affichées (`apiKey`, `projectId`, …) dans `config.js`.
5. Sur GitHub : **Settings → Pages → Deploy from a branch → main / (root)**.
   Le planning est en ligne à l'adresse `https://automultiservices.github.io/planning-atelier/`.

## Limites
- Pas de comptes : toute personne qui a le lien peut voir et modifier le planning. Ne partagez le lien qu'en interne.
- Le code commercial évite les erreurs de manipulation, ce n'est pas une sécurité.
- La lecture des BL se fait sur le texte du PDF : un BL scanné (image) doit être saisi avec « Créer un BL sans PDF ».
