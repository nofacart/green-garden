# 🌿 Mon Jardin Connecté

Application web statique pour suivre l’état hydrique du potager, des plantes ornementales et de la pelouse, directement dans le navigateur.

Cette version a été refondée pour fonctionner sans backend, avec un stockage local, des prévisions météo et des recommandations orientées jardinage.

## ✨ Ce que fait l’application

- Suivi du jardin en direct via les prévisions Open-Meteo.
- Tableau de bord de synthèse avec : cultures actives, prochain arrosage et prochaine tonte.
- Calcul de l’état hydrique du sol et suivi du déficit accumulé.
- Prédiction d’arrosage adaptée à la météo, au type de sol et aux cultures suivies.
- Prédiction de tonte en fonction de la hauteur du gazon et du seuil configuré.
- Gestion détaillée des cultures avec dates de plantation et d’arrachage.
- Paramétrage de la localisation du jardin et du type de sol.
- Saisie d’arrosages manuels avec date et quantité en litres.
- Système de goutte à goutte automatique programmable.
- Historique des interventions et journal d’actions.
- Graphiques dynamiques du déficit hydrique avec Chart.js.
- Sauvegarde locale dans le navigateur via LocalStorage.
- Export / import de sauvegarde JSON vers le stockage cloud ou le système de fichiers.

## 🚀 Démarrage rapide

1. Ouvrir le fichier [index.html](index.html) dans un navigateur moderne.
2. Utiliser l’onglet “Direct du jour” pour obtenir la synthèse du jardin.
3. Définir la localisation, le type de sol et les cultures dans l’onglet “Réglages”.
4. Saisir les interventions (arrosage manuel, tonte, goutte à goutte) pour alimenter les calculs.
5. Exporter ou importer les données si vous souhaitez synchroniser votre jardin entre appareils.

## 🧠 Fonctionnement principal

L’application combine plusieurs sources de données pour proposer une décision simple et rapide :

- météo locale pour les pluies et températures prévues ;
- besoins spécifiques des plantes selon leur catégorie et leur cycle ;
- type de sol pour ajuster la capacité de rétention d’eau ;
- historique d’arrosage et de tonte pour calculer le déficit hydrique.

Le résultat est une interface orientée action qui aide à décider si le jardin doit être arrosé, si la pelouse peut attendre, ou si un entretien est à prévoir.

## 🔄 Sauvegarde et synchronisation

Le projet est 100 % local, sans serveur backend.

- Sur ordinateur, le bouton d’export permet d’écrire directement dans un dossier synchronisé (OneDrive, Google Drive, Dropbox, iCloud, etc.).
- Sur mobile ou sur les navigateurs plus limités, l’application génère un fichier JSON standard à enregistrer manuellement.
- L’import recharge immédiatement les données pour restaurer ou synchroniser un jardin entre appareils.

## 📁 Structure du projet

- [index.html](index.html) : interface principale de l’application et logique du jardin.
- [README.md](README.md) : présentation et documentation utilisateur.
- [CHANGELOG.md](CHANGELOG.md) : historique des évolutions du projet.

## 📝 Historique des évolutions

Le détail des changements récents est documenté dans [CHANGELOG.md](CHANGELOG.md).

## 🛠️ À venir

Le projet reste orienté vers un usage pratique et local, avec des améliorations possibles sur :

- le raffinement des seuils agronomiques ;
- les recommandations de culture selon les observations réelles ;
- l’amélioration des éléments visuels et de lisibilité sur l’onglet principal.