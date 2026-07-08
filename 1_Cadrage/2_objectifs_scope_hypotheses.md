# Objectifs, scope et hypothèses

## 1. Objectifs SMART

### 1.1 Mise en ligne rapide

Permettre à un restaurateur de créer et publier son site vitrine et son menu digital en moins de 30 minutes, dans 90% des cas, dès la première utilisation de la plateforme.

### 1.2 Adoption du QR code

Atteindre un taux d’utilisation du menu via QR code supérieur à 40% des clients dans les établissements équipés, dans les 3 mois suivant le déploiement.

### 1.3 Activation des restaurateurs

Obtenir au moins 70% des restaurateurs actifs (ayant créé un menu et généré un QR code) dans les 7 jours suivant leur inscription.

### 1.4 Utilisation de la commande sur place

Atteindre un taux d’utilisation de la fonctionnalité de commande sur place par QR code d’au moins 25% des clients dans les 3 mois suivant le lancement.

### 1.5 Engagement produit

Permettre à plus de 50% des restaurateurs de modifier leur menu au moins une fois par semaine.

## 2. Périmètre IN

*Le MVP inclut les fonctionnalités suivantes :*

- Création d’un site vitrine pour le restaurant
- Gestion des informations et médias du restaurant
- Gestion de la carte
- Génération de QR codes (global et par table)
- Consultation du menu via QR code
- Commande sur place
- Gestion du service
- Gestion des salles et des tables
- Gestion des rôles et du staff
- Paramétrage du restaurant
- Gestion du profil utilisateur
- Consultation des statistiques d’activité

## 3. Périmètre OUT 

*Le MVP n’inclut pas les fonctionnalités suivantes :*

- Gestion de paiement en ligne ou sur place
- Intégration avec des systèmes de caisse
- Gestion comptable
- Gestion RH avancée
- Gestion de livraison
- Marketplace ou plateforme B2C
- Automatisation marketing avancée
- Benchmark entre restaurants


Le périmètre du MVP est volontairement limité afin de garantir une mise en oeuvre rapide et une adoption facilitée par les restaurateurs.

Les éléments exclus du périmètre MVP pourront être intégrés dans des phases ultérieures, en fonction des retours utilisateurs et des priorités produit.

## 4. Hypothèses

*Le projet repose sur les hypothèses suivantes :*

| **Hypothèses** | **Justification** | **Risque si invaliditée** | **Criticité** |
| --- | --- | --- | --- |
| Une part suffisante des clients utilisera le QR code pour justifier le déploiement de la solution | Usage des QR codes largement démocratisé post-COVID dans la restauration | Si faible adoption : valeur produit réduite pour le restaurateur, désengagement | ÉLEVÉE |
| Les clients sont suffisamment à l’aise avec les smartphones pour utiliser la solution sans assistance | Taux d'équipement smartphone élevé en France (\>80% des adultes) | Expérience dégradée pour une partie de la clientèle, friction à l’adoption | MOYENNE |
| Les restaurateurs ciblés sont prêts à payer un abonnement SaaS pour digitaliser leur présence | Hypothèse pas encore validée | Modèle économique non viable, besoin de revoir le pricing ou le modèle de distribution | ÉLEVÉE |
| Le besoin de digitalisation des restaurants indépendants est structurel et durable | Accélération de la transformation digitale dans la restauration post-COVID (Banque de France, rapport numérique restauration) | Marché moins porteur que prévu | FAIBLE |
| La mise en ligne complète est réaliste en moins de 30 minutes dès la première utilisation | Objectif de conception explicite du produit, onboarding simplifié | Abandon à l’onboarding, taux d’activation faible, réputation négative | ÉLEVÉE |
| La commande sur place sans paiement apporte une valeur suffisante pour être activée par les restaurateurs | Hypothèse fragile : certains restaurateurs pourraient la juger incomplète sans encaissement | Fonctionnalité peu utilisée, effort de développement non rentabilisé | MOYENNE |
| La solution n’est pas soumise à la certification NF525 (caisse enregistreuse) car elle ne gère pas l’encaissement | Choix stratégique explicite du CDC : hors périmètre paiement et encaissement certifié | Obligation légale non respectée, risque juridique majeur, refonte nécessaire | ÉLEVÉE |
| Le MVP peut être livré par une équipe réduite dans un délai raisonnable sans dette technique excessive | Périmètre volontairement limité, stack technique choisie pour sa rapidité de développement | Retards, dette technique, périmètre réduit ou qualité dégradée au lancement | MOYENNE |
