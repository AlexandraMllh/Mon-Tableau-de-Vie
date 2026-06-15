# 🌿 Mon Tableau de Vie

Dashboard personnel PWA (Progressive Web App) — accessible depuis n'importe quel appareil, installable sur l'écran d'accueil, fonctionne hors-ligne.

🔗 **[Ouvrir l'app](https://alexandramallah.github.io/Mon-Tableau-de-Vie)**

---

## ✨ Fonctionnalités

### 📅 Aujourd'hui
- Navigation jour par jour (passé / futur)
- **Météo** en temps réel (Open-Meteo, sans clé API) — géolocalisation auto **ou ville saisie et mémorisée**
- Anneaux de progression des habitudes
- Humeur, sommeil (horaires + qualité), énergie
- **🤰 Mal de ventre** (estomac/intestins) **et 🩸 endométriose** (utérus) — deux jauges distinctes
- **🍽️ Alimentation du jour** — repas + calories, ajout direct d'une recette (portions + ingrédients auto)
- **💊 Suivi pilule** — bouton à cocher, streak affiché
- **🧪 Balance des hormones** — dopamine, sérotonine, ocytocine, endorphines déduites de tes activités, repas, moments sociaux, soins et accomplissements (tâches **et jalons** terminés)
- To-do du jour
- Journal / routines

### 💼 Travail
- Projets & tâches (avec jalons pondérés, priorité, avancement, glisser-déposer)
- **🤖 Pour Claude** — coche un jalon « pour Claude » → il s'affiche dans une liste dédiée sous le calendrier des deadlines
- Bilan hebdo / mensuel
- Candidatures, articles, communications
- **⏱️ Gestion du temps** — saisie par catégorie, stats **cette semaine** (navigation ◀ ▶) / ce mois (depuis le 1er), graphiques 14 j & 30 j
- **🚆 Missions pro postdoc** — train / repas / taxi / essence / **péage**, remboursements (états), budget ; un **frais pro peut alimenter automatiquement** une ligne de mission
- **📓 Notes** — groupes, éditeur WYSIWYG (gras, italique, titres, listes…)
- Réseau / CRM

### 🏃 Activités
- Suivi des séances sportives semaine par semaine
- Planning sport
- Graphique 14 jours

### 🩺 Santé
- Composition corporelle (poids, masse grasse, masse maigre)
- **🔥 Apport calorique 30 jours** — graphe + **moyennes de la semaine et du mois** (jours renseignés)
- Hydratation quotidienne
- Bien-être sur 30 jours
- **💜 Corrélations bien-être** — réseau visuel reliant sommeil, énergie, humeur, mal de ventre et endométriose (corrélations de Pearson)
- Routines (skincare…) — streak et calendrier 30 jours
- **💊 Suivi pilule** — calendrier 90 jours, streak, record, % du mois
- Pas quotidiens
- Tendances & prédictions

### 💰 Finances
- Comptes courant & épargne avec soldes automatiques
- Transactions (dépenses, revenus, épargne, hors compte, frais pro)
- Catégories personnalisées (**ajout / suppression** directement depuis le menu) + catégories pro automatiques
- **💼 Frais pro & remboursements** — suivi des états (lancé / reçu), montant remboursé ≠ dépensé, répartition courant/hors compte, détection du surplus ; rattachement possible aux **missions postdoc**
- Jauge budget mensuel
- **📉 Évolution du solde** — courbe sur 90 jours
- **⚖️ Comparaison mois N vs N-1** — dépenses / revenus / épargne / hors compte
- Flux 6 derniers mois
- Répartition par catégorie
- Prévisions & abonnements

### 🍽️ Domestique
- To-do du jour (partagé avec Aujourd'hui)
- **🍳 Recettes** — ingrédients avec calories, total + **par portion**, catégories pastel, filtre par kcal (préréglages + plage perso), recherche, emoji auto ou manuel
- **Planning repas** — clic sur un créneau pour éditer, ou 📖 pour piocher une recette (par nom / catégorie / kcal)
- Liste de courses (par événement)
- 🌱 Plantes — fréquence d'arrosage, alertes, détection depuis Google Agenda

### 📅 Calendrier
- Vue mensuelle interactive
- Import ICS (Google Agenda, etc.)
- Synchronisation Google Agenda via URL iCal
- Événements manuels
- Intégration des tâches, jalons, abonnements, plantes

### 📔 Journal
- Journal quotidien libre
- Mots-clés humeur détectés automatiquement

### 🧱 Piliers de vie
- Suivi de 8 piliers (santé, travail, finances, loisirs…)
- Score hebdomadaire avec métriques automatiques cliquables (détail des événements pris en compte)

### ⚙️ Réglages & sauvegarde
- Prénom, habitudes, activités, catégories (dépenses / revenus / épargne), charges fixes, soldes de départ, types de candidatures
- **💾 Exporter / Importer mes données** — sauvegarde `.json` datée (changement d'appareil, de navigateur, ou récupération si l'adresse du site change)

> ⚠️ Les données vivent dans le **navigateur** (localStorage), cloisonnées par adresse du site. **Exporter régulièrement** est le meilleur filet de sécurité.

---

## 🚀 Installation sur mobile

1. Ouvre `alexandramallah.github.io/Mon-Tableau-de-Vie` dans **Samsung Internet** ou **Chrome**
2. Menu → **Ajouter à l'écran d'accueil**
3. L'app s'installe comme une vraie application, fonctionne hors-ligne

---

## 🔧 Stack technique

| Élément | Détail |
|---|---|
| Frontend | HTML / CSS / JS vanilla — fichier unique `index.html` |
| Graphiques | Chart.js 4 |
| Sync cloud | Firebase Firestore (auth Google) |
| Stockage local | `localStorage` |
| PWA | Service Worker network-first, cache offline |
| Hébergement | GitHub Pages |
| Météo | [Open-Meteo](https://open-meteo.com) (gratuit, sans clé) |
| Géocodage | [Nominatim](https://nominatim.org) (OpenStreetMap) |

---

## 🔄 Mises à jour

Les mises à jour sont **automatiques** — l'app se recharge toute seule quand une nouvelle version est disponible (toast "🔄 Mise à jour — rechargement…").

Le numéro de version est visible dans le titre de l'onglet (ex. `v402`).
