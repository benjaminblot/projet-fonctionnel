# Risques initiaux

## 1. Matrice de risques

| **PROBABILITÉ / IMPACT** | **IMPACT FAIBLE** | **IMPACT MOYEN** | **IMPACT ELEVEE** |
| --- | --- | --- | --- |
| **PROBABILITÉ FAIBLE** |  |   | - RGPD - Perte de données  |
| **PROBABILITÉ MOYENNE** | - Faible utilisation commande | - Problèmes techniques - Dépendance comportement client - Bug menu - Retards intégrations techniques - Collecter des stats fiables | - Faible adoption QR code - Réticence restaurateurs |
| **PROBABILITÉ ELEVEE** |   |  | - Complexité dev  |

---

## 2. Détails des risques et mesures de mitigation

### 2.1 Faible adoption du QR code par les clients

- *Description :* les clients pourraient ne pas utiliser le QR code, réduisant l’utilité de la solution pour le restaurateur.
- *Mesures de mitigation :* interface simple et intuitive, affichage clair du QR code sur place, communication via le restaurateur (explication rapide à la clientèle), suivi statistiques des scans pour identifier les obstacles.

### 2.2 Réticence des restaurateurs à adopter la solution

- *Description :* certains restaurateurs pourraient être hésitants à utiliser une nouvelle plateforme Saas.
- *Mesures de mitigation :* onboarding rapide ( \< 30 min), démonstration de la valeur concrète (SEO local, menu digital, gain de temps…), support dédié pour faciliter la prise en main.

### 2.3 Problèmes techniques (perfomance mobile, affichage, réseau…)

- *Description :* l’application pourrait rencontrer des bugs ou des lenteurs sur mobile, affectant l’expérience utilisateur.
- *Mesures de mitigation :* optimisation mobile, tests en conditions réelles sur différents terminaux, architecture légère, monitoring post-lancement.

#### 2.4 Complexité du développement

- *Description :* les fonctionnalités prévues pourraient prendre plus de temps à développer que prévu, retardant le MVP.
- *Mesures de mitigation :* découpage clair du MVP en user stories, priorisation stricte des fonctionnalités essentielles, suivi quotidien de l’avancement avec l'équipe dev.

### 2.5 Faible utilisation de la commande sans paiement

- *Description :* la fonctionnalité de commande sur place pourrait être peu utilisée par les clients, réduisant l’intérêt de cette feature.
- *Mesures de mitigation :* communication claire aux clients lors de l’expérience sur place, suivi des statistiques, possibilité de proposer une intégration de paiement dans une phase ultérieure.

### 2.6 Dépendance au comportement des clients (usage smartphone)

- *Description :* le projet dépend de l’usage des smartphones par les clients, ce qui peut varier selon le type de clientèle.
- *Mesures de mitigation :* maintien d’un alternative papier si nécessaire, test pilote pour évaluer l’usage, adaptation progressive selon les retours.

### 2.7 Bugs ou erreurs sur le menu digital 

- *Description :* le menu digital pourrait contenir des erreurs (prix, allergènes, disponibilité), impactant l’expérience client et la crédibilité du restaurateur.
- *Mesures de mitigation :* tests unitaires, QA avant mise en production, possibilité de corrections rapides.

### 2.8 Retards liés aux intégrations techniques

- *Description :* l’intégration des QR codes oud es notifications pourraient prendre plus de temps que prévu.
- *Mesures de mitigation :* planification détaillées des intégrations, tests préalables, communication régulière avec les fournisseurs ou modules tiers.

### 2.9 Problèmes de sécurité / RGPD

- *Description :* non-respect des règles RGPD ou vulnérabilités pourraient entraîner des sanctions ou perte de confiance.
- *Mesures de mitigation :* gestion des accès par rôle, mentions légales, définition de la durée de conservation des données, cookies, politique de confidentialité, sauvegarde et localisation des données encadrées, tests de sécurité avant production.

### 2.10 Difficulté à collecter des statistiques fiables

- *Descritpion :* les statistiques sur l’usage des menus et commandes pourraient être incomplètes ou erronées.
- *Mesures de mitigation :* définition claire des KPI, test sur échantillon pilote, monitoring en continu.

### 2.11 Perte de données ou crash serveur

- *Description :* risque de perte de données ou indisponibilité du service.
- *Mesures de mitigation :* sauvegardes régulières, hébergement sécurisé, plan de reprise après incident, monitoring serveur.
