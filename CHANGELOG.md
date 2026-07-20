# Changelog

Toutes les modifications notables de ce projet sont documentées ici.

## [Unreleased]

### À venir
- Affinage du comportement de prédiction pour les cultures et la pelouse.
- Ajustements de la logique agronomique selon les retours d’usage réel.
- Amélioration visuelle des composants de décision sur l’onglet principal.

## [1.1.0] - 2026-07-20

### Ajouts
- Nouveau tableau de bord de synthèse sur l’onglet principal.
- Résumé des actions à venir : plantes actives, prochain arrosage et prochaine tonte.
- Intégration des prévisions météo directement dans le suivi du jour.
- Gestion des cultures avec dates de plantation et d’arrachage.
- Prédiction de l’arrosage à partir des prévisions de température et de pluie.
- Prédiction de la tonte en fonction de la hauteur de pelouse et des seuils configurés.
- Paramétrage utilisateur de la localisation du jardin pour adapter les prévisions météo.
- Paramétrage du type de sol pour ajuster les besoins en eau estimés.
- Enregistrement d’un arrosage manuel avec date personnalisable et quantité en litres.
- Apport standard recommandé affiché dynamiquement selon le type de sol choisi.

### Améliorations
- Réduction de la friction UX sur l’onglet de suivi.
- Cohérence renforcée entre les cartes de synthèse, le météo et le graphique du déficit hydrique.
- Ajout de boutons de réinitialisation ciblés pour l’hydrique, le journal et les données complètes.
- Mise à jour du résumé principal pour afficher le contexte du jardin actif.

### Corrections
- Correction de la cohérence des valeurs affichées entre le résumé et les séries de déficit.
- Simplification de la logique d’affichage des cultures actives ou hors période selon les dates saisies.
- Correction du flux de saisie de l’arrosage pour conserver une date et une quantité d’eau réalistes.
