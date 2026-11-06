# Planning Atelier AMS

Planning hebdomadaire de l'atelier : les commerciaux déposent les BL (PDF) et les placent sur la semaine,
l'atelier consulte le planning, coche « Terminé » et envoie des notes aux commerciaux.
Tout est synchronisé en direct entre tous les appareils.

- Accès commercial : bouton « Accès commercial », code **4567**.
- Vue atelier : par défaut, pour tout le monde.
- Bouton « Exporter en PDF » (accès commercial) : planning de la semaine affichée en A4 paysage, plus la liste des BL à planifier en page 2. Pratique pour partager le planning par mail.

## En ligne
- Planning : https://automultiservices.github.io/planning-atelier/
- Base de données : projet Firebase `ams-planning` (console.firebase.google.com), Firestore en Europe (eur3).
- Règles de la base : fichier `firestore.rules` (à recoller dans Firestore → Règles en cas de modification).

## Limites
- Pas de comptes : toute personne qui a le lien peut voir et modifier le planning. Ne partagez le lien qu'en interne.
- Le code commercial évite les erreurs de manipulation, ce n'est pas une sécurité.
- La lecture des BL se fait sur le texte du PDF : un BL scanné (image) doit être saisi avec « Créer un BL sans PDF ».
