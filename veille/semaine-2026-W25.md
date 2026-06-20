# Idées outils – Semaine 2026-W25

---

## 1. Comparateur de flux de déchets par commune

**Quoi** : Script qui agrège les tonnages de collecte par commune et par flux (OMR, tri, verre, carton) depuis les exports Excel de l'exutoire, et génère un tableau comparatif avec évolution N-1 et écart à la moyenne intercommunale.

**Stack** : Python (pandas) + Excel/Power Query

**Gain** : Identifier rapidement les communes en décrochage ou en progrès pour orienter les actions de communication et les ajustements de dotation en PAV.

---

## 2. Carte de chaleur des signalements PAV

**Quoi** : Carte Leaflet qui visualise la densité et la nature des signalements terrain (dépôts sauvages, vandalisme, débordement) sur une période glissante, avec filtres par type et par commune.

**Stack** : HTML/JS + Leaflet.js + Leaflet.heat + CSV/GeoJSON

**Gain** : Prioriser les interventions de maintenance, détecter les secteurs récurrents pour y renforcer la sensibilisation ou revoir l'implantation.

---

## 3. Outil de suivi des marchés et prestataires PAV

**Quoi** : Page HTML standalone avec tableau de bord des marchés actifs (prestataire, date de fin, montant, prochaine révision de prix, contacts) et alertes visuelles J-90 / J-30 avant échéance.

**Stack** : HTML/JS + localStorage (aucune dépendance serveur)

**Gain** : Ne plus rater une reconduction ou un renouvellement de marché, centraliser les informations dispersées dans les emails et dossiers partagés.

---

## 4. Extracteur de données cadastrales pour implantation PAV

**Quoi** : Script Python qui, à partir d'une liste de parcelles candidates, interroge l'API Carto (IGN/Géoportail) pour récupérer propriétaire, surface, nature et génère un tableau prêt pour les demandes d'autorisation d'occupation.

**Stack** : Python (requests) + API Carto / data.gouv.fr

**Gain** : Réduire de plusieurs heures la phase administrative d'identification foncière lors de chaque nouvelle implantation.

---

## 5. Simulateur de rentabilité auto-école

**Quoi** : Outil HTML/JS qui calcule le chiffre d'affaires prévisionnel selon le nombre d'élèves, le mix de formations (B, AAC, code seul, BSR) et les tarifs, avec seuil de rentabilité et projection mensuelle sur 12 mois.

**Stack** : HTML/JS + Chart.js (standalone, hors ligne)

**Gain** : Aide à la décision pour ajuster les tarifs ou la capacité d'accueil, préparation rapide des prévisions pour le bilan comptable ou un prêt.

---

*Généré automatiquement le 2026-06-20 (semaine ISO 25)*
