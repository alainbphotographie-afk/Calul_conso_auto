# Calcul coût du trajet

Application web permettant de calculer le coût d’un trajet selon :
- le type de carburant
- le prix au litre
- la distance
- la consommation moyenne

## Lien de l'application
https://alainbphotographie-afk.github.io/Calul_conso_auto/

## Historique des modifications

### v1
- Calcul manuel du coût du trajet.
- Sélection E98, E95 et Diesel.

### v2
- Correction de l’affichage mobile.
- Suppression du bouton calcul redondant.

### v3
- Champs distance et consommation laissés vides par défaut.

### v4
- Ajout de la récupération automatique des prix via l’API officielle.

### v5
- Modification du comportement de l’API pour récupérer la station la plus proche au lieu de la moins chère dans un rayon de 15 km.

### V6
-Cette version utilise l’API publique Opendatasoft des prix des carburants et un géocodage OpenStreetMap/Nominatim pour le mode manuel, ce qui correspond bien à la logique que tu veux mettre en place pour afficher la station la plus proche. Si tu veux une version 100% calée sur ton ancien fichier existant avec le même design, les mêmes champs trajet/consommation et sans rien casser visuellement, colle-moi ton index.html actuel dans le prochain message
