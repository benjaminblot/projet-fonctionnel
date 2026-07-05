# Plan de test

## 1. Contexte et objectifs 

| **Projet** | Plateforme SaaS vitrine digitale et menu QR  pour restaurateurs |
| --- | --- |
| **Objectif** | Valider que les fonctionnalités MVP développées répondent aux critères d’acceptation définis dans les user stories et aux besoins métier des trois personas identifiés |
| **Type de tests** | Tests fonctionnels (UAT), hors tests techniques et tests de sécurité avancés |
| **Version testée** | MVP v1.0 |

## 2. Périmètre

| | | 
| --- | --- |
| **Dans le périmètre** | - Toutes les US Must : authentification, restaurant, QR code, carte, expérience client, service, gestion opérationnelle - Scénarios utilisateurs |
| **Hors périmètre** | - US Should, Could et Won’t non livrées en MVP - Tests de performance - Tests de sécurité avancés  - Tests sur navigateurs non listés ci-dessous |

## 3. Acteurs et responsabilités

| | |
| --- | --- |
| **Rédaction de tests** | BA / AMOA |
| **Exécution des tests** | BA / AMOA |
| **Correction des anomalies** | Développeur |
| **Validation finale ** | Product owner |

## 4. Environnement de test

| | |
| --- | --- |
| **Environnement** | Environnement de recette (staging) |
| **Navigateurs testés** | - Chrome desktop (dernière version) - Safari mobile iOS (iPhone) - Chrome mobile Android |
| **Données de test** | Jeu de données fictif |

## 5. Épics et user stories couverts

| **Épic** | **User stories couvertes** | **Priorité** |
| --- | --- | --- |
| EP-01 Authentification | - Créer un compte - Se connecter - Se déconnecter - Modifier son mot de passe - Réinitialiser son mot de passe | MUST |
| EP-02 Restaurant | - Créer son établissement - Modifier les informations de son restaurant - Publier / dépublier son restaurant - Gérer les salles et les tables | MUST |
| EP-03 Carte | - Gérer les cartes - Gérer les menus - Gérer les plats - Publier / dépublier un menu | MUST |
| EP-04 QR code | - Générer un QR code global - Générer un QR code par table | MUST |
| EP-05 Expérience client | - Consulter le menu via QR code - Consulter la page vitrine d’un restaurant - Passer une commande | MUST |
| EP-06 Service | - Ouverture / fermeture du service - Consulter les commandes en temps réel - Mettre à jour le statut d’une commande | MUST |
| EP-06 Gestion opérationnelle | - Paramétrer le restaurant - Gérer le staff | MUST |

## 6. Critères de sortie de recette

| | |
| --- | --- |
| **Critère de succès** | 100% des cas de test Must en statut “Pass” |
| **Critère d'échec** | Au moins 1 cas de test Must en statut “Fail” bloquant non résolu |
| **Gestion des anomalies** | Toute anomalie bloquante est remontée dans Jira avec priorité “High”, correction obligatoire avant mise en production. Les anomalies mineures sont documentées et planifiées en itération suivante |
