# Planning Atelier AMS

Planning hebdomadaire de l'atelier : les commerciaux déposent les BL (PDF) et les placent sur la semaine,
l'atelier consulte le planning, coche « Terminé » et envoie des notes aux commerciaux.
Tout est synchronisé en direct entre tous les appareils.

- Accès commercial : bouton « Accès commercial », code **4567**.
- Vue atelier : par défaut, pour tout le monde.

## En ligne
- Planning : https://automultiservices.github.io/planning-atelier/
- Base de données : projet Firebase `ams-planning` (console.firebase.google.com), Firestore en Europe (eur3).
- Règles de la base : fichier `firestore.rules` (à recoller dans Firestore → Règles en cas de modification).

## Limites
- Pas de comptes : toute personne qui a le lien peut voir et modifier le planning. Ne partagez le lien qu'en interne.
- Le code commercial évite les erreurs de manipulation, ce n'est pas une sécurité.
- La lecture des BL se fait sur le texte du PDF : un BL scanné (image) doit être saisi avec « Créer un BL sans PDF ».
