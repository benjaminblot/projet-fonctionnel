# Justification des choix

## 1. Justification du périmètre MVP

### 1.1 Pourquoi se concentrer sur une vitrine et la commande via QR code

*Double objectif business identifié dès le cadrage :*

Le business case identifie deux problèmes distincts mais liés : l’absence de visibilité en ligne des restaurateurs et la digitalisation insuffisante de l’expérience client en salle. Traiter un seul des deux problèmes aurait limité la valeur perçue par le restaurateur. Un menu digital sans visibilité en ligne n’attire pas de nouveaux clients, une vitrine sans commande digitale ne modernise pas l’expérience en salle.


*Cohérence avec les personas et user journeys : *

Les trois personas de Marc, Julie et Thomas représentent chacun une étape différente du parcours complet. Exclure l’un des deux piliers aurait laissé un persona sans utilité réelle dans le produit. Sans vitrine, Marc ne résout pas son problème de visibilité, sans commande, Julie et Thomas ne bénéficient pas de l’amélioration de l’expérience en salle.

### 1.2 Pourquoi exclure le paiement intégré du MVP

*Réduction de la complexité réglementaire : *

L’intégration d’un paiement en ligne implique la norme NF525 des obligations de certification lourdes (cf. hypothèse H7 du document de cadrage). Cette contrainte aurait considérablement allongé le temps de développement et complexifié le MVP, allant à l’encontre de l’objectif de mise en ligne rapide qui est un KPI central du projet.


*Validation du besoin avant l’investissement technique :* 

L’hypothèse H6 (commande sans paiement) identifiée dans le document Cadrage souligne que la valeur de cette fonctionnalité n’est pas encore validée auprès des restaurateurs. Investir dans une intégration paiement avant d’avoir confirmé l’adoption de la commande sur place aurait représenté un risque de développement non rentabilisé.

### 1.3 Pourquoi prioriser la gestion des rôles 

*Sécurité fonctionnelle minimale dès le lancement : *

La séparation des rôles garantit qu’un membre du staff ne peut accéder aux paramètres sensibles du restaurant. Dès qu’un restaurant emploie plusieurs personnes, ce qui est la norme même pour un petit établissement, l’absence de contrôle d’accès représente une faille de sécurité incompatible avec un usage réel, même en MVP.

### 1.4 Pourquoi intégrer la gestion du service dans le MVP

*Différenciateur produit fort :*

La gestion du service répond directement au pain point opérationnel des restaurateurs identifié dans les personas et le CDC. Sans cette fonctionnalité, le restaurateur ne peut pas contrôler quand et comment les clients accèdent à la commande, ce qui représente un risque opérationnel et de fraude incompatible avec un déploiement réel.


*Cohérence avec le périmètre commande sur place :*

La commande sur place sans gestion du service reviendrait à laisser les QR codes actifs en permanence, y compris en dehors des heures d’ouverture. La gestion du service est donc une dépendance fonctionnelle du pilier “commande sur place” défini comme Must.

## 2. Justification des arbitrages MoSCoW

### 2.1 Gérer les salles et tables

- *Aurait pu être :* should (perçue comme un raffinement de la commande)
- *Justification :* la commande sur place dépend structurellement de l’identification de la table via QR code (cf. business rules 6.1 et 8.1). Sans gestion des tables, l’association automatique commande/table décrite dans le CDC est techniquement impossible. Cette US est donc une dépendance technique du Must “Passer une commande”, pas une fonctionnalité de confort.

### 2.2 Consulter la page vitrine d’un restaurant

- *Aurait pu être :* should (perçue comme secondaire par rapport au menu)
- *Justification :* cette US sert directement le premier pilier du MVP (la visibilité en ligne). Le persona Marc n’atteint son objectif principal (exister en ligne) que si sa page vitrine est consultable. La retirer viderait le premier objectif business de toute valeur concrète pour le restaurateur.

### 2.3 Modifier la carte du service

- *Aurait pu être :* must (l’offre varie selon les services dans la restauration réelle)
- *Justification :* en MVP strict, un restaurateur peut fonctionner avec une carte fixe par service sans que cela bloque le parcours de commande. La flexibilité de modifier la carte en cours de service est un différenciateur opérationnel fort qui améliore significativement l’adoption. Cette fonctionnalité est donc prioritaire en phase post-MVP mais non bloquante pour le lancement.

### 2.4 Supprimer son compte

- *Aurait pu être :* must (obligation RGPD)
- *Justification :* le droit à l’effacement (article 17 RGPD) est une obligation légale mais peut être géré manuellement par l'équipe en phase de MVP. La fonctionnalité doit être livrée rapidement après le lancement mais ne bloque pas la mise en production initiale.

### 2.5 Suivre le statut de sa commande (client)

- *Aurait pu être :* must (cohérence avec la promesse de transparence du parcours client)
- *Justification :* le client est physiquement présent en salle et peut constater l’avancement de sa commande sans interface dédiée (cf. analyse persona Julie). Cette US améliore significativement l’expérience mais n’est pas bloquante pour que le flux de sa commande fonctionne de bout en bout. Le staff peut traiter la commande même sans que le client suive son statut en temps réel.

### 2.6 Gérer ses allergènes (profil client)

- *Aurait pu être :* must (enjeu de sécurité alimentaire)
- *Justification :* les allergènes sont déjà affichés sur chaque plat (cf. Business rule 5.6), le client peut les consulter sans compte. La personnalisation des allergènes dans le profil est un confort supplémentaire, pas une obligation de sécurité bloquante pour le MVP.

### 2.7 Consulter ses récapitulatifs de commandes

- *Aurait pu être :* should (fonctionnalité valorisée par le client)
- *Justification :* cette US dépend d’un compte client connecté, lui même optionnel dans le parcours. Elle ajoute de la complexité réglementaire (données personnelles historisées) pour une fonctionnalité non essentielle à la proposition de valeur du MVP. Candidate naturelle pour la phase 2 cependant.
