# CAHIER DES CHARGES 
# Plateforme de vitrine digitale et menu QR pour restaurateurs

## 1. Contexte et objectif du projet

### 1.1 Objectif principal 
Créer une plateforme SaaS B2B permettant aux restaurateurs : 
- D'avoir un site vitrine 
- D'améliorer leur référencement local
- De proposer un menu digital via QR code
- De permettre une commande sur place simple
- De visualiser des statistiques utiles sans remplacer la caisse ni gérer des contraintes réglementaires lourdes.

---

### 1.2 Cible
- Restaurateurs indépendants
- Bars, brasseries, cafés
- Restaurants sans site web ou avec site obsolète
- Établissements souhaitant un menu QR simple et efficace


## 2. Périmètre fonctionnel 

### 2.1 Site vitrine restaurant


**Objectif**

Permettre à chaque restaurant de disposer d'une page web publique, hébergée sur la plateforme, visible en ligne et accessible via une URL unique. Les restaurants sont indexables et accessibles via une page de recherche publique par nom et par localisation.


**Fonctionnalités**

- Gestion des informations du restaurant
- Gestion des actualités et événements
- Recherche publique du restaurant

**Contraintes**

- Page responsive optimisée pour mobile
- URL publique propre et indexable
- Optimisation SEO local
- Chargement rapide

---

### 2.2 Carte digitale et QR code

**Objectif**

Permettre au restaurateur de créer et gérer sa carte digitale selon une hiérarchie Carte → Menu → Plat, accessible par les clients via QR code sans installation d'application.

**Fonctionnalités** 

- Gestion des cartes
- Gestion des plats
- Organisation des plats par catégories
- Recherche de plat par catégorie
- Gestion de la disponibilité des plats
- Publication et dépublication d'une carte ou d'un menu
- Génération de QR codes dynamiques
- Téléchargement des QR codes
- Impression ou export PDF de la carte des allergènes

**Contraintes**

- Accès au menu sans installation d'app mobile
- Chargement de la page menu en moins de 3 secondes
- Interface lisible sans zoom sur mobile
- QR code unique par restaurant et par table

---

### 2.3 Commande sur place via QR 

**Objectif**

Permettre au client de commander depuis son téléphone, sans gestion d'encaissement certifié. La commande est automatiquement associée à la table identifiée par le QR code scanné.

**Fonctionnalités** 

- Gestion des plats dans le panier 
- Suivi du statut de la commande
- Notification client
- Mise à jour du statut de la commande
- Archivage des commandes terminées

**Contraintes**

- Mise à jour visible en moins de 5 secondes
- Aucune commande possible si service fermé

---

### 2.4 Gestion des salles et des tables

**Objectif**

Permettre au restaurateur de contrôler l'ouverture et la fermeture du service, d'adapter la carte proposée et de gérer le plan de table en temps réel.

**Fonctionnalités** 

- Ouverture et fermeture du service
- Sélection ou modification de la carte avant ou pendant le service
- Gestion des salles et des tables
- Historique de commandes par table
- Historique des services passés

**Contraintes**

- Tables et commandes inaccessibles aux clients lorsque le service est fermé
- Modification du plan de table disponible uniquement durant un service actif

---

### 2.5 Gestion des rôles et du staff

**Objectif**

Permettre à l'administrateur de contrôler les accès de chaque membre du staff selon un système de rôles configurables.

**Fonctionnalités**

- Administrateur : Accès complet, gestion de la carte, des tables, du staff, des paramètres et des statistiques
- Serveur : Consultration et mise à jour des commandes en cours, modification du plan de table
- Invité : À définir par l'administrateur

Globalement, les rôles ci-dessus sont générés par défaut, ils sont modifiables en amont par l'administrateur. Les fonctionnalités de ce module sont : 
- Gestion des utilisateurs
- Gestion des rôles
- Configuration des droits associés à chaque rôle par l'administrateur

**Contraintes**

- Fonctionnalités disponibles uniquement si associées à un rôle ou un utilisateur
- Modification des droits réservée à l'administrateur

---

### 2.6 Paramétrage du restaurant

**Objectif**

Permettre à l'administrateur d'adapter le comportement de la plateforme aux spécificités de son établissement.

**Fonctionnalités**

- Définition de la devise pour l'affichage des prix
- Définition du fuseau horaire
- Activation ou désactivation de la prise de commande en ligne
- Configuration de l'ouverture automatique du service selon des horaires définis
- Activation du code d'accès salle
- Gestion des langues disponibles pour l'affichage du menu

**Contraintes**

- Paramètres accessibles uniquement par l'administrateur
- Modifications applicables immédiatement sans redémarrage

---

### 2.7 Statistiques et analytics

**Objectif**

Fournir au restaurateur des données simples, lisibles et orientées action pour comprendre et optimiser son activité, sans exposer de données personnelles identifiables.

**Fonctionnalités**

- Statistiques journalières
- Statistiques par service

**Contraintes**

- Données agrégées, aucune donnée personnelle identifiable exposée
- Accessibles uniquement par l'administrateur par défaut
- Données mises à jour régulièrement et correspondant à l'activité du jour en cours

## 3. Périmètre non inclus (volontairement)
- Caisse enregistreuse 
- Gestion de paiement certifiée
- Comptabilité
- Gestion RH complète
- Benchmark inter-restaurants
- Marketplace / guide B2C
- Livraison
- Logistique

## 4. Parcours utilisateurs

### 4.1 Restaurateur
1. Inscription
2. Création de son établissement
3. Configuration de la page vitrine
4. Création de la carte
5. Création des salles et tables
6. Génération des QR codes
7. Paramétrage du restaurant
8. Gestion du staff et des rôles
9. Ouverture du service
10. Consultation des statistiques

---

### 4.2 Client final
1. Scan du QR code
2. Sélection de la langue (optionnel)
3. Consultation de la page vitrine
4. Consultation du menu
5. Commande sur place
6. Suivi du statut de la commande
7. Consultation de l'historique (si connecté)

---

### 4.3 Staff
1. Connexion à l'interface staff
2. Consultation des commandes en temps réel
3. Mise à jour du statut d'une commande
4. Modification du plan de table
5. Fermeture du service

## 5. Exigences techniques

### Architecture
- Frontend : React / Next.js
- Backend : Java
- Base de données : Postgresql
- Infrastructure : Kubernetes
- Hébergement : VPS
- Notifications : Email
- QR codes : Génération dynamique

## 6. Sécurité et conformité
- Données sécurisées
- Accès par rôle
- RGPD :
    - Mentions légales
    - Cookies
    - Durée de conservation des données 
    - Droit à l'effacement
    - Localisation des données
    - Politique de confidentialité distincte des mentions légales
    - Distinction responsable de traitement (plateforme) et sous-traitant (restaurateur pour les données clients)
- Sauvegarde régulière

## 7. MVP / priorités

### MVP indispensable
1. Site vitrine
2. Menu digital
3. QR codes
4. Commande sur place 
5. Vue staff
6. Statistiques basiques

---

### A faire plus tard
- Paiement
- Multilingue avancé
- Intégrations externes
- Automatisation marketing

## 8. Indicateurs de succès 
- Temps de mise en ligne inférieur à 30 min
- Utilisation QR par les clients supérieure à 60% 
- Restaurateurs actifs hebdomadaires (au moins une action significative) supérieur à 40%
- Fréquence de mise à jour semestrielle des menus supérieure à 40%
- Commandes via QR supérieur à 30%
- Adoption QR côté restaurant : 60% ayant activé au moins un QR code à M+1

## 9. Evolution future (roadmap)

### Phase 2
- Paiement en ligne optionnel
- Intégration réservations externes
- Exports données
- Automatisations simples
- Menus multilingues

---

### Phase 3 
- Benchmark inter-restaurateurs
- IA recommendations
- Multi-établissements 

## 10. Conclusion
Ce projet est :
- Cohérent
- Bien cadré
- Faisable avec une équipe réduite
- Utile immédiatement
- Évolutif sans dette excessive

**Très bonne base produit.** 

