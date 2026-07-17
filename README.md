# 🌿 Mon Jardin Connecté

Application web statique et ultra-rapide pour le suivi hydrique du potager et de la pelouse à Beauzelle. 

Anciennement propulsé par Streamlit, ce projet fonctionne désormais à 100 % dans le navigateur pour garantir une indépendance et une confidentialité totale des données.

## ✨ Caractéristiques
- **Suivi en direct :** Intégration de l'API Open-Meteo pour récupérer pluies et températures sans clé d'API.
- **Calcul intelligent :** Moteur d'estimation du déficit en eau du sol mis à jour automatiquement.
- **Graphiques natifs :** Évolution dynamique via Chart.js.
- **Zéro Base de données serveur :** Tout est stocké de manière sécurisée dans votre navigateur (`LocalStorage`).

## 🚀 Installation & Déploiement
1. Hébergé gratuitement via **GitHub Pages**.
2. Utilisable instantanément sur Mobile ou Desktop.

## 🔄 Sauvegarde et Synchronisation Cloud

L'application est 100% locale, mais elle intègre désormais une gestion intelligente des sauvegardes grâce à l'**API File System Access** :

* **Sur Ordinateur (Chrome, Edge, Opera) :** Le bouton "Exporter" ouvre l'explorateur natif de votre système. Vous pouvez sélectionner directement un dossier synchronisé (*Google Drive, OneDrive, Dropbox, iCloud*) et écraser votre ancien fichier `jardin_backup.json` pour éviter d'accumuler des doublons.
* **Sur Mobile / Safari / Firefox :** L'application génère un fichier `.json` standard et sollicite le système d'exploitation (iOS/Android) pour vous permettre de le ranger dans votre application *Fichiers* ou *Drive*.
* **Importation :** Le bouton "Importer" permet de charger instantanément ce même fichier pour synchroniser vos données sur un autre appareil.