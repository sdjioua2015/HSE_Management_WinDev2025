# Logiciel de Gestion HSE - WinDev 2025 / Client-Serveur

Ce dépôt contient un socle de projet pour un logiciel de gestion HSE (Hygiène, Sécurité, Environnement) en architecture Client/Serveur, conçu pour être développé sous WinDev 2025 avec SQL Server.

## Objectif

Le logiciel vise à centraliser la gestion des:
- incidents et accidents
- audits et inspections
- actions correctives
- personnel et habilitations
- risques et conformité
- documents et procédures
- rapports et statistiques

## Architecture proposée

- Client : application WinDev 2025
- Serveur de données : SQL Server
- Modèle : Client/Serveur avec accès centralisé aux données
- Sécurité : connexion utilisateur + profils + droits par module
- Rapports : PDF, export Excel, tableaux de bord

## Modules principaux

- Authentification
- Gestion des entreprises et sites
- Gestion du personnel
- Gestion des incidents
- Gestion des audits
- Gestion des actions correctives
- Gestion des formations et habilitations
- Gestion des risques
- Documentation / procédures
- Rapports et statistiques
- Administration et logs

## Structure du dépôt

- `database/` : script SQL de création de la base HSE
- `src/WinDev/` : exemples de code WLanguage pour les fenêtres WinDev
- `mockups/` : maquettes graphiques SVG des fenêtres principales
- `docs/` : documentation fonctionnelle

## Base de données

Fichier : `database/HSE_DB.sql`

Elle contient :
- tables d’entreprise, sites, départements
- profils et utilisateurs
- personnel
- incidents et gravité
- audits et points d’audit
- actions correctives
- formations
- documents
- risques
- logs

## Exemple de fenêtres WinDev 

Les écrans ci-dessous sont fournis sous forme de maquettes visuelles (SVG), afin de donner une idée fidèle du rendu attendu dans WinDev :

- Login
- Accueil / Tableau de bord
- Gestion des incidents

Fichiers dans `mockups/`.

## Exemples de code WLanguage

Les fichiers de code dans `src/WinDev/` démontrent :
- connexion à la base
- validation du login
- ouverture du menu principal
- ajout d’un incident
- chargement d’une grille

## Démarrage rapide

1. Créer la base SQL Server
2. Exécuter le script `database/HSE_DB.sql`
3. Ouvrir WinDev 2025
4. Créer le projet applicatif
5. Importer les écrans et codes de `src/WinDev/`
6. Ajuster la chaîne de connexion au serveur
7. Tester la connexion et les écrans

## Sécurité recommandée

- mot de passe hashé
- profils par utilisateur
- droits par module
- journalisation des actions
- validation des données saisies
- contrôle des suppressions

## Remarques

Ce projet est une base solide de démarrage, pensée pour être évolutive. Il peut être complété par :
- génération PDF
- envoi de notifications
- API REST
- statistiques avancées
- reporting dynamique
- synchronisation multi-sites

## Licence

Projet de démonstration / prototype de gestion HSE.

## Auteur

Projet généré pour un besoin de gestion HSE en environnement WinDev 2025.
