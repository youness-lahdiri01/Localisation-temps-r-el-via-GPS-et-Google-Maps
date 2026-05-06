# Real-Time Location Tracking App (GPS + Google Maps + PHP + MySQL)
## Description

Cette application Android permet de suivre la localisation en temps réel d’un utilisateur en utilisant le GPS et d’afficher sa position sur une carte Google Maps.

Le projet repose sur une architecture complète :

## Application Android (GPS + envoi des coordonnées)
## Backend PHP (API REST)
## Base de données MySQL (stockage des positions)

## L’intégration de la carte est réalisée avec le Maps SDK for Android fourni par Google.

## Objectifs du projet
Récupérer la position GPS en temps réel
Envoyer les coordonnées vers un serveur distant
Stocker les positions dans une base MySQL
Afficher les positions sur Google Maps
Comprendre l’architecture client / serveur
## Technologies utilisées
## Mobile
Java
Android Studio
Google Maps SDK for Android
Volley (requêtes HTTP)
GPS / Location Services
## Backend
PHP
API REST
## Base de données
MySQL
## Serveur local
XAMPP / WAMP / LAMP
## Installation
1. Cloner le projet
git clone https://github.com/youness-lahdiri01/Localisation-temps-r-el-via-GPS-et-Google-Maps.git
## Configuration
🔹 1. Backend (PHP + MySQL)
Lancer XAMPP / WAMP
Placer le dossier backend dans :
htdocs/
Créer une base de données MySQL (ex: gps_db)
Importer le fichier .sql (si موجود)
🔹 2. Réseau

## IMPORTANT :

Le téléphone et le PC doivent être sur le même réseau Wi-Fi
Utiliser l’adresse IP locale du PC (ex: 192.168.x.x)
🔹 3. Android
Ouvrir le projet dans Android Studio
Synchroniser Gradle
🔹 4. 🔑 Ajouter la clé API Google Maps

👉 Ce projet NE contient PAS de clé API Google Maps.

Pour des raisons de sécurité, aucune clé API n’est fournie.

Créer une clé ici :
👉 https://console.cloud.google.com/

Puis l’ajouter dans :

app/src/main/res/values/google_maps_api.xml
<string name="google_maps_key">VOTRE_CLE_API</string>
📱 Fonctionnalités
📍 Récupération de la position GPS en temps réel
📡 Envoi des coordonnées vers le serveur (PHP API)
🗄️ Stockage dans MySQL
🗺️ Affichage des positions sur Google Maps
🔄 Mise à jour continue de la localisation
🔄 Fonctionnement global
L’application récupère la position GPS
Elle envoie latitude & longitude via HTTP (Volley)
Le serveur PHP reçoit et stocke dans MySQL
L’application récupère les positions
Affichage sur Google Maps avec markers
<img width="425" height="851" alt="Screenshot 2026-05-06 174306" src="https://github.com/user-attachments/assets/006d21c4-2f8b-4565-8b4b-0cbbc4fcf15b" />



<img width="517" height="858" alt="Screenshot 2026-05-06 174316" src="https://github.com/user-attachments/assets/f049b056-672b-4484-a1ab-12e848d40dec" />

## Remarques importantes
Sans clé API → la carte ne fonctionne pas
Vérifier les permissions GPS
Vérifier la connexion réseau
L’API PHP doit être accessible depuis le téléphone
## Problèmes fréquents
❌ Carte grise → clé API manquante
❌ Aucune position → problème GPS ou permissions
❌ Erreur réseau → IP incorrecte ou serveur non lancé
❌ Données non enregistrées → erreur MySQL / PHP
## Auteur

Youness LAHDIRI

## Licence

Projet éducatif – utilisation libre pour apprentissage
