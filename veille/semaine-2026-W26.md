# Idées outils – Semaine 2026-W26

## 1. Carte interactive PAV hors ligne

**Quoi** : Page HTML standalone affichant tous les PAV de la NCPA sur une carte Leaflet, filtrable par commune et par type (colonnes enterrées, cabines carton, aires de collecte), avec export PDF de la vue courante.

**Stack** : HTML/JS + Leaflet.js + GeoJSON statique + html2canvas

**Gain** : Support visuel prêt pour les réunions avec les élus, utilisable sans connexion une fois la page ouverte, sans serveur à maintenir.

---

## 2. Générateur de fiches d'incident PAV

**Quoi** : Script Python qui lit un CSV d'incidents (exporté depuis QField) et génère automatiquement une fiche PDF par signalement — identifiant PAV, type d'incident, photo attachée, date — avec QR code renvoyant vers la fiche du point sur la carte.

**Stack** : Python + reportlab + qrcode + pandas

**Gain** : Standardise les remontées terrain, facilite le suivi avec le prestataire de collecte, crée un historique archivable sans outil tiers.

---

## 3. Optimiseur de tournées de collecte

**Quoi** : Script Python qui prend en entrée les coordonnées GPS des PAV et leur fréquence de remplissage, calcule un ordre de passage optimisé par tournée, et exporte un fichier CSV + GeoJSON prêt à charger dans QField ou Google Maps.

**Stack** : Python + GeoPandas + OR-Tools (Google) ou nearest-neighbor simple

**Gain** : Réduit les kilomètres parcourus à vide par le prestataire, argument chiffrable pour les bilans environnementaux de l'intercommunalité.

---

## 4. Tableau de suivi des taux de collecte par commune

**Quoi** : Script Python + Power Query qui agrège les données de pesée par commune et par flux (verre, carton, biodéchets), calcule l'évolution mensuelle et produit un tableau Excel mis en forme avec sparklines et alertes de seuil.

**Stack** : Python + openpyxl (ou directement Power Query M)

**Gain** : Indicateurs clés disponibles en quelques secondes après réception des données du prestataire, sans retraitement manuel.

---

## 5. Rapport mensuel auto-école (auto-école Bayonne)

**Quoi** : Script Python qui lit un CSV de gestion (recettes, élèves, examens du mois) et génère un PDF de 1 page résumant le CA, le nombre d'élèves actifs, le taux de réussite permis B, et un graphe d'évolution sur 12 mois.

**Stack** : Python + pandas + matplotlib + reportlab

**Gain** : Vision mensuelle consolidée en moins d'une minute, sans saisie manuelle dans Excel, reproductible d'un mois sur l'autre.
