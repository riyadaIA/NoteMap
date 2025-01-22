# NoteMate

NoteMate est une application Android permettant aux étudiants de prendre, organiser et partager leurs notes de manière intuitive. Elle offre une solution à la fois accessible hors ligne et synchronisée en ligne, permettant ainsi une expérience fluide et collaborative.

## Table des matières

- [Introduction](#introduction)
- [Fonctionnalités](#fonctionnalités)
- [Conception](#conception)
- [Aspects techniques](#aspects-techniques)
- [Données](#données)
- [Intégrations](#intégrations)
- [Planification](#planification)
- [Livraison et maintenance](#livraison-et-maintenance)

## Introduction

### Contexte du projet

L'objectif de l'application est de faciliter la gestion des notes pour les étudiants et enseignants de CEFOD Business School. Elle permet aux étudiants de prendre des notes en classe, de les organiser par matière et de les partager avec d'autres utilisateurs.

### Objectifs de l'application

- Prendre des notes structurées par catégorie.
- Partager les notes avec d'autres utilisateurs.
- Accès hors ligne avec sauvegarde locale.
- Synchronisation des données avec Firebase pour une collaboration en temps réel.

### Public cible

Étudiants et enseignants de **CEFOD Business School**.

### Nom provisoire de l'application

**NoteMate**

---

## Fonctionnalités

### Fonctionnalités principales

- **Authentification** : Connexion avec Firebase Authentication.
- **Gestion des notes** : Création, modification, suppression et organisation par matière.
- **Partage** : Partage des notes avec d'autres utilisateurs.
- **Synchronisation** : Sauvegarde en Firebase et accès hors ligne via SQLite.

### Fonctionnalités secondaires

- Notifications de mise à jour des notes partagées.
- Thème clair et sombre pour personnalisation de l'interface.

---

## Conception

### Interface Utilisateur (UI)

- **Maquettes** : Écran de connexion, tableau de bord, éditeur de note.
- **Charte graphique** : Bleu (#1E90FF), Blanc (#FFFFFF), Gris clair (#F5F5F5).
- **Typographie** : Roboto.
- **Ergonomie** : Interface intuitive et accessible.

### Expérience Utilisateur (UX)

**Cas d'utilisation** :

1. L'étudiant crée une note, la sauvegarde hors ligne et la partage ensuite.
2. Consultation des notes partagées.

---

## Aspects techniques

### Plateforme

- **Système d'exploitation** : Android (version minimale : Android 8.0).

### Technologies

- **Langage** : Java.
- **Framework** : Android Jetpack.
- **Base de données** :
  - Locale : SQLite.
  - En ligne : Firebase Realtime Database.
  
### Architecture

- **Modèle** : MVVM (Model-View-ViewModel).

---

## Données

### Données à gérer

- **Texte** : Notes, sous-titres, paragraphes.
- **Images** : Illustrations dans les notes.
- **Informations utilisateur** : Nom, prénom, email.

### Synchronisation des données

- Synchronisation entre SQLite et Firebase lors de la connexion.

---

## Intégrations

- **Firebase Authentication** : Gestion des utilisateurs.
- **Firebase Realtime Database** : Stockage des notes partagées.

---

## Planification

### Ressources

- 1 développeur mobile.
- 1 designer UI/UX.
- 1 chef de projet.

---

## Livraison et maintenance

- **Déploiement** sur Google Play Store.
- **Documentation utilisateur**.
- **Support technique** et mises à jour régulières.

---

## Annexes

- **Maquettes** : Écrans de l'application.
- **Diagrammes** : Flux utilisateur et modèle de données.

---

### Entités principales

1. **Utilisateur** : Informations sur l'utilisateur (id, nom, prénom, email, etc.).
2. **Catégorie (Matière)** : Organisation des notes par matière (id, nom, description).
3. **Note** : Notes créées par les utilisateurs (id, titre, description).
4. **NotePart** : Parties de la note (sous-titres, paragraphes, images).
