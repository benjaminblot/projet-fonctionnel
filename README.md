# Business Analyst Project — Plateforme SaaS QR Menu

## Contexte du projet

Ce dossier présente l'ensemble des livrables fonctionnels produits dans le cadre d'un projet de groupe dont la partie technique est développée en parallèle. L'objectif est de démontrer une maîtrise opérationnelle des méthodes et outils utilisés par un Business Analyst, Product Owner ou PMO junior en contexte professionnel.

Le projet consiste en une plateforme SaaS B2B permettant aux restaurateurs indépendants de digitaliser leur présence en ligne et leur expérience client en salle via un système de menu QR code et commande sur place.

## Structure du dossier

```text
/business-analyst-project
│
├── README.md
├── Cahier_des_charges.md
│
├── 1_Cadrage/
│ ├── 1_business_case.md
│ ├── 2_objectifs_scope_hypotheses.md
│ └── 3_risques_initiaux.md
│
├── 2_Parties_prenantes/
│ ├── 1_stakeholder_map.md
│ └── 2_matrice_raci.md
│
├── 3_Analyse_existant/
│ ├── 1_user_journey_restaurateur.md
│ ├── 2_user_journey_client_final.md
│ ├── 3_user_journey_staff.md
│ └── 4_process_as_is.pdf
│
├── 4_Conception/
│ ├── 1_vision_produit.md
│ ├── 2_user_stories.md
│ ├── 3_business_rules.md
│ └── 4_process_to_be.pdf
│
├── 5_Priorisation/
│ ├── 1_priorisation_moscow.pdf
│ └── 2_justification_choix.md
│
├── 6_Recette/
│ ├── 1_plan_de_test.md
│ ├── 2_cas_de_test.md
│ └── 3_scenarios_utilisateurs.md
│ 
└── 7_Annexes/
  └── 1_grid_power_interest.pdf
```

## Contenu des livrables

### 1. Cadrage
- Business case : contexte marché, problème, solution, bénéfices attendus, KPI cibles et conclusion décisionnelle
- Objectifs, scope et hypothèses : objectifs SMART, périmètre IN/OUT du MVP, hypothèses structurées avec justification, criticité et plan de validation
- Risques initiaux : matrice probabilité/impact, détail des 11 risques identifiés avec mesures de mitigation

### 2. Parties prenantes
- Stakeholder map : cartographie des parties prenantes selon la matrice pouvoir/intérêt
- Matrice RACI : activités réparties dans différentes phases projet, avec rôles distincts

### 3. Analyse de l'existant
- User journeys : 3 parcours avec persona détaillé, analyse avec implication produit et tableau user journey
- Process AS-IS : modélisation BPMN du processus de commande existant avec annotation des points de friction

### 4. Conception
- Vision produit : positionnement, problème, cible, solution, proposition de valeur, différenciation et vision long terme
- User stories : 40+ US réparties en différents epics avec critères d'acceptation testables (export jira)
- Business rules : différents domaines fonctionnels couverts, cohérents avec la hiérarchie de la carte
- Process TO-BE : modélisation BPMN du processus de commande cible

*Les wireframes ont été réalisés au cours du projet mais ne sont pas publiés dans ce dossier. Ils sont intégrés directement dans l'environnement de développement. Les use cases n'ont pas été produits : le niveau de détail des user stories et des business rules couvre l'essentiel de ce qu'apporterait cet artefact dans ce contexte.*

### 5. Priorisation
- Priorisation MoSCoW : répartition des US avec visuel à 4 colonnes
- Justification des choix : justification du périmètre MVP et justification des arbitrages MoSCoW les plus discutables

*Le backlog produit a été intégralement géré sous Jira : epics, user stories, critères d'acceptation et priorisation MoSCoW y sont disponibles. L'export natif Jira ne permettant pas de générer un PDF lisible directement, le backlog n'est pas inclus comme livrable dans ce dossier. La priorisation MoSCoW est disponible sous forme de synthèse visuelle.*

### 6. Recette
- Plan de test : stratégie de recette, périmètre, acteurs, environnement, epics couverts et critères de sortie
- Cas de test UAT : 18 cas de test couvrant l'epic *Authentification* à titre d'exemple représentatif, avec préconditions, étapes détaillées et résultats attendus
- Scénarios utilsiateurs : 3 scénarios de bout en bout couvrant le cycle complet *inscription → service → commande → traitement*

*Les cas de test présentés couvrent un seul epic à titre d'exemple représentatif de la méthodologie appliquée. Les critères d'acceptation de l'ensemble des US Must ont été rédigés et sont disponibles dans le document de user stories. Une couverture complète des cas de test sera réalisée avant toute mise en production.*

### 7. Annexes
- Certains visuels de référence utilisés dans les livrables principaux. Ces éléments sont référencés directement depuis les documents concernés.

## Livrables non inclus

### Suivi et pilotage
Les livrables de suivi : tableau de bord KPI, suivi des risques et dépendances, roadmap n'ont pas été formalisés dans ce dossier. Le suivi a été réalisé de manière informelle au fil de l'avancement, via des échanges directs avec l'équipe technique et des ajustements ponctuels du backlog Jira. Les éléments de cadrage (KPI cibles, risques initiaux, vision roadmap) sont disponibles respectivement dans le business case, le document de risques initiaux et la vision produit.

## Outils utilisés
- Jira : gestion du backlog et des user stories
- Confluence : documentation fonctionnelle
- Lucidchart : modélisation des processus AS-IS et TO-BE (BPMN)
- Figma : wireframes
- Xray : gestion des cas de test

## Profil
Diplômé d'un Master MIAGE, ce dossier a été réalisé dans l'objectif de démontrer une capacité opérationnelle immédiate sur des postes de BA, PO, PMO ou AMOA, sans nécessiter de formation complémentaire significative.
