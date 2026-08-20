# Changelog

Toutes les modifications notables de ce projet sont documentées ici.

## [Unreleased]

### À venir
- Raffinement de la logique agronomique selon les retours d’usage réel.
- Ajustements éventuels sur les seuils et recommandations de tonte.
- Améliorations visuelles et ergonomiques sur les écrans de décision.

## [1.3.0] - 2026-08-20

### Ajouts
- Modèle agronomique avancé avec courbe de température pour calculer le coefficient de besoin en eau.
- Système d'évapotranspiration de référence (ET0) pour affiner les prédictions de déficit hydrique.
- Calcul d'efficacité de la pluie : les pluies supérieures au seuil sont comptabilisées avec un coefficient réduit pour modéliser le ruissellement.
- Suivi du stade de croissance des plantes (jeune vs mature) avec facteur de réduction du besoin en eau pour les jeunes cultures.
- Gestion du paillage avec facteur de réduction automatique du déficit hydrique.
- Migration intelligente des anciennes cultures ornementales vers une gestion générique.

### Améliorations
- Calcul du déficit hydrique plus proche des réalités agronomiques et climatiques.
- Prédictions plus justes selon la saison et le stade de développement des cultures.
- Meilleure prise en compte de la pluviométrie réelle vs efficace.

### Corrections
- Nettoyage automatique des données ornementales légacy lors du premier démarrage en v1.3+.

## [1.2.2] - 2026-08-18

### Améliorations
- Ajout d’un badge visuel de statut sur le programme de goutte-à-goutte pour distinguer clairement le mode actif et inactif.
- Clarification du message de validation lorsque le programme est enregistré mais n’est pas encore activé.
- Alignement de l’affichage du déficit hydrique sur les volumes en litres pour améliorer la lecture et la cohérence visuelle.

### Corrections
- Correction de la logique d’historique versionné du goutte-à-goutte pour conserver les passages passés et reprendre correctement le bon programme à partir de sa date de référence.
- Stabilisation du calcul d’irrigation automatique quand plusieurs réglages sont enregistrés à des dates différentes.
- Vérification du bon recalcul du déficit hydrique après une modification du programme d’arrosage automatique.

## [1.2.1] - 2026-08-17

### Corrections
- Correction de la logique d’historique versionné du goutte-à-goutte pour conserver les passages passés et reprendre correctement le bon programme à partir de sa date de référence.
- Stabilisation du calcul d’irrigation automatique quand plusieurs réglages sont enregistrés à des dates différentes.
- Vérification du bon recalcul du déficit hydrique après une modification du programme d’arrosage automatique.

## [1.2.0] - 2026-08-17

### Ajouts
- Système de goutte à goutte automatique avec activation, zones desservies, fréquence et date de référence.
- Gestion avancée des cultures avec ajout, suppression et suivi des périodes de plantation / arrachage.
- Tableau de bord de synthèse plus riche sur l’onglet de suivi.
- Journal d’interventions détaillé pour les arrosages, tonte et autres actions.
- Export / import de sauvegarde JSON via le système de fichiers ou un dossier synchronisé dans le cloud.
- Contrôle du statut hydrique du sol et suivi visuel du déficit accumulé.

### Améliorations
- Intégration complète des prévisions météo dans le parcours de décision du jour.
- Recommandations de volume d’arrosage calculées à partir du déficit accumulé et du type de sol.
- Mise à jour de l’UX des réglages avec configuration du jardin, des zones et des cultures.
- Cohérence renforcée entre le résumé principal, le graphique hydrique et les conseils de gestion.
- Ajout de reset ciblés pour l’hydrique, le journal et les données complètes.

### Corrections
- Correction de la logique d’affichage des cultures actives selon leurs périodes validées.
- Validation plus robuste des entrées de date et de quantité d’arrosage.
- Normalisation du stockage des paramètres de jardin et de l’état hydrique local.
- Correction du comportement de sélection et de calcul sur les zones de culture / pelouse.

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
