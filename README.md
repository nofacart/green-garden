# 🌿 Mon Jardin Connecté

Application web statique et ultra-rapide pour le suivi hydrique du potager et de la pelouse.

Anciennement propulsée par Streamlit, cette version fonctionne entièrement dans le navigateur pour préserver la confidentialité des données et éviter tout besoin de backend.

## ✨ Ce que fait l’application
- **Suivi de jardin en direct :** utilisation d’Open-Meteo pour récupérer les prévisions de pluie et les températures.
- **Tableau de bord orienté action :** résumé des cultures actives, du prochain arrosage et de la prochaine tonte.
- **Prédictions intelligentes :** estimation du prochain arrosage à partir des températures et des pluies prévues.
- **Prédiction de tonte :** suivi de la hauteur du gazon et estimation de l’intervention à venir.
- **Gestion détaillée des cultures :** dates de plantation et d’arrachage pour tenir compte des périodes actives/inactives.
- **Graphiques dynamiques :** suivi visuel du déficit hydrique via Chart.js.
- **Sauvegarde locale :** stockage des données dans le navigateur avec LocalStorage.
- **Export / import :** gestion d’une sauvegarde JSON via l’API File System Access lorsqu’elle est disponible.

## 🚀 Utilisation
1. Ouvrir le fichier [index.html](index.html) dans un navigateur moderne.
2. Utiliser l’onglet “Direct du jour” pour contrôler les décisions du jour.
3. Gérer les cultures et les dates depuis l’onglet Réglages.
4. Exporter ou importer les données si besoin pour synchroniser entre appareils.

## 🔄 Sauvegarde et synchronisation cloud

L’application est 100 % locale, mais elle prend en charge des sauvegardes manuelles via l’API File System Access :

- **Sur ordinateur (Chrome, Edge, Opera) :** le bouton “Exporter” ouvre l’explorateur système pour choisir un dossier synchronisé comme OneDrive, Google Drive, Dropbox ou iCloud.
- **Sur mobile / Safari / Firefox :** l’application génère un fichier JSON standard à placer dans votre espace de fichiers.
- **Importation :** le bouton “Importer” recharge immédiatement la sauvegarde pour restaurer ou synchroniser vos données.

## 📝 Historique des évolutions

Le détail des changements récents est documenté dans [CHANGELOG.md](CHANGELOG.md).