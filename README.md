# ⛽ Calcul Coût du Trajet

Une application web **mobile-first** pour calculer le coût en carburant d'un trajet, avec récupération automatique des prix à la pompe via géolocalisation.

---

## 📸 Aperçu

> Interface épurée, responsive, conçue pour une utilisation rapide sur smartphone ou ordinateur.

---

## ✨ Fonctionnalités

- 🔴 **Géolocalisation** : détecte votre position et interroge l'API officielle du gouvernement français pour trouver les prix des carburants dans un rayon de 15 km
- ⛽ **3 carburants supportés** : E98, E95 (SP95), Diesel
- 💾 **Persistance locale** : les prix et le carburant sélectionné sont sauvegardés via `localStorage`
- 🧮 **Calcul instantané** : affichage du coût total avec le détail du calcul (litres consommés × prix/L)
- 📍 **Affichage de la station** : nom, adresse et ville de la station la plus avantageuse affichés après récupération
- ✅ **Validation des saisies** : message d'erreur si les valeurs sont manquantes ou invalides

---

## 🗂️ Structure du projet

```
├── index.html   # Application complète (HTML + CSS + JavaScript en un seul fichier)
```

L'application est **entièrement contenue dans un seul fichier** `index.html`, sans dépendance externe ni framework.

---

## 🚀 Utilisation

1. Ouvrez `index.html` dans un navigateur moderne (Chrome, Firefox, Safari, Edge)
2. Cliquez sur **📍 Récupérer les prix près de moi** et autorisez la géolocalisation
3. Sélectionnez votre carburant (E98, E95 ou Diesel)
4. Saisissez la **distance** en km et votre **consommation** en L/100 km
5. Le coût du trajet s'affiche instantanément

> 💡 Les prix peuvent aussi être saisis manuellement si la géolocalisation n'est pas disponible.

---

## 🌐 API utilisée

Les prix des carburants sont récupérés en temps réel depuis l'API officielle du gouvernement français :

**[Prix des carburants en France – Flux instantané v2](https://data.economie.gouv.fr/explore/dataset/prix-des-carburants-en-france-flux-instantane-v2/)**

```
https://data.economie.gouv.fr/api/explore/v2.1/catalog/datasets/
prix-des-carburants-en-france-flux-instantane-v2/records
```

La requête filtre les stations dans un rayon de **15 km** et sélectionne celle proposant le **Diesel le moins cher** avec le maximum de carburants disponibles.

---

## 🛠️ Technologies

| Technologie | Usage |
|---|---|
| HTML5 | Structure de la page |
| CSS3 | Mise en page responsive, animations, dégradés |
| JavaScript (Vanilla ES6+) | Logique applicative, appels API, localStorage |
| Geolocation API (Web) | Récupération de la position utilisateur |
| Open Data Gouvernement FR | Prix des carburants en temps réel |

---

## 📱 Compatibilité

- ✅ Chrome / Edge (desktop & mobile)
- ✅ Safari (iOS & macOS)
- ✅ Firefox
- ✅ Tout navigateur moderne supportant la **Geolocation API**

---

## 📄 Licence

Ce projet est distribué sous licence **MIT**. Vous êtes libre de l'utiliser, le modifier et le redistribuer.

---

## 👤 Auteur

Développé par **Alain B** – Île-de-France, France
