# Gestion des Commandes - Application Pizzeria

## Description

Cette application mobile est conçue pour aider une pizzeria à gérer ses commandes reçues par message, offrir une interface rapide et visuelle pour surveiller les commandes en cours, et fournir des outils de gestion de la caisse. L'application est destinée à être utilisée uniquement en interne sur une tablette.

---

## Fonctionnalités principales

- **Gestion des commandes** :

  - Ajout, modification et suppression des commandes.
  - Affichage en temps réel des commandes en cours.

- **Interface utilisateur intuitive** :

  - Design adapté pour une utilisation sur tablette.
  - Accès rapide aux commandes en attente et terminées.

- **Gestion de la caisse** :

  - Suivi des paiements (espèces, CB, autres).
  - Calcul des totaux journaliers et export des données.

- **Stockage local** :

  - Aucune connexion Internet requise.
  - Les données sont stockées directement sur la tablette.

- **Export de données** :

  - Export des commandes et des journaux de caisse au format CSV.

---

## Technologies Utilisées

- **Frontend et Backend** :

  - [Flutter](https://flutter.dev/) (Dart) pour une application multiplateforme fluide.

- **Base de données locale** :

  - SQLite avec l'intégration de [Drift](https://drift.simonbinder.eu/) pour une gestion facile des données.

- **Design UI** :

  - Material Design pour une interface moderne et ergonomique.

---

## Prérequis

1. Une tablette Android.
2. [Flutter SDK](https://flutter.dev/docs/get-started/install) installé sur votre machine de développement.
3. [Android Studio](https://developer.android.com/studio) pour tester et compiler l'application.

---

## Installation et Déploiement

### 1. Cloner le dépôt :

```bash
git clone https://github.com/votre-repo/gestion-commandes-pizzeria.git
cd gestion-commandes-pizzeria
```

### 2. Installer les dépendances :

Assurez-vous que Flutter est configuré correctement, puis exécutez :

```bash
flutter pub get
```

### 3. Tester sur un appareil ou un émulateur :

Lancez l'application sur un appareil connecté ou un émulateur Android :

```bash
flutter run
```

### 4. Générer un APK pour déploiement :

Pour déployer l'application sur la tablette :

```bash
flutter build apk --release
```

Le fichier APK se trouvera dans le dossier `build/app/outputs/flutter-apk/`.

### 5. Installer l'APK sur la tablette :

Transférez et installez l'APK sur la tablette via USB ou en utilisant un outil comme ADB :

```bash
adb install build/app/outputs/flutter-apk/app-release.apk
```

---

## Structure du Projet

- `lib/` : Contient le code source de l'application.

  - `main.dart` : Point d'entrée de l'application.
  - `screens/` : Les différents écrans (commandes, caisse, tableau de bord).
  - `models/` : Les modèles de données (Commande, Paiement).
  - `database/` : Gestion de la base de données locale avec SQLite.

- `assets/` : Ressources statiques (images, icônes).

- `test/` : Tests unitaires et d'intégration.

---

## Prochaines Étapes

- Ajouter des notifications pour signaler de nouvelles commandes.
- Intégrer une fonctionnalité de rapport statistique (ventes hebdomadaires, mensuelles).
- Améliorer la personnalisation de l'interface utilisateur.

---

## Contribution

Les contributions sont les bienvenues ! Merci de suivre ces étapes :

1. Fork le dépôt.
2. Créer une branche pour vos modifications :
   ```bash
   git checkout -b feature/nouvelle-fonctionnalite
   ```
3. Soumettre une pull request.

---

## Licence

Ce projet est sous licence MIT. Voir le fichier `LICENSE` pour plus d'informations.

