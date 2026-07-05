# Scénarios utilisateurs

## 1. Scénario 1 - Marc : de l’inscription à l’ouverture du service

| **Persona** | Marc, restaurateur indépendant, 45 ans |
| --- | --- |
| **Objectif** | Valider que Marc peut créer son compte, configurer son restaurant, créer une carte, générer ses QR codes et ouvrir son premier service en moins de 30 minutes |
| **Préconditions** | Aucun compte existant, accès depuis un ordinateur |
| **Étapes** | 1. Marc crée son compte avec un email et un mot de passe valides 2. Il valide son inscription avec le code reçu par mail 3. Il se connecte et accède à son tableau de bord 4. Il crée son restaurant avec le nom, l’adresse et les horaires 5. Il publie son restaurant pour le rendre visible en ligne 6. Il crée une carte “Carte du midi” avec un menu et 3 plats (nom + prix) 7. Il publie sa carte 8. Il génère le QR code global et un QR code pour la table 1 9. Il paramètre son restaurant (devise, fuseau horaire) 10. Il ouvre manuellement le service |
| **Résultat attendu** | Le restaurant est visible en ligne, la carte est consultable via QR code, le service est actif et les commandes sont possibles, durée totale inférieure à 30 minutes |

## 2. Scénario 2 - Julie : consultation, allergènes et commande

| **Persona** | Julie, cliente restaurant, 28 ans, connectée à son compte avec un allergène (gluten) renseigné |
| --- | --- |
| **Objectif** | Valider que Julie peut accéder au menu, être alertée sur ses allergènes, choisir ses plats et passer commande depuis son smartphone |
| **Préconditions** | Restaurant et carte publiés, service ouvert, QR code par table actif, Julie est assise à la table 3 et connectée à son compte |
| **Étapes** | 1. Julie scanne le QR code de la table 3 2. La carte s’affiche sur son smartphone dans sa langue préférée 3. Elle parcourt les plats, ceux contenant du gluten sont signalés visuellement 4. Elle sélectionne deux plats sans gluten 5. Elle consulte son panier et valide la commande 6. Elle reçoit une confirmation et suit le statut de sa commande |
| **Résultat attendu** | La commande est transmise au staff, la table 3 est automatiquement identifiée, les plats contenant du gluten étaient clairement signalés avant sélection |

## 3. Scénario 3 - Thomas : traitement des commandes pendant le service

| **Persona** | Thomas, serveur, 24 ans |
| --- | --- |
| **Objectif** | Valider que Thomas peut accéder au dashboard, consulter les commandes en temps réel, mettre à jour leur statut et gérer une fusion de tables en cours de service |
| **Préconditions** | Thomas est connecté à l’interface staff, le service est ouvert, au moins une commande est en attente sur la table 3 |
| **Étapes** | 1. Thomas accède au dashboard commandes 2. Il consulte la commande de la table 3 3. Il passe le statut de “Envoyée” à “En préparation” 4. Une table supplémentaire rejoint le groupe, Thomas fusionne la table 3 et la table 4 en ajustant la capacité de cette nouvelle table 5. La cuisine prépare la commande, Thomas passe le statut à “Prête” 6. Il apporte les plats et passe le statut à “Servie” |
| **Résultat attendu** | Chaque changement de statut est sauvegardé immédiatement, la fusion de tables regroupe automatiquement les commandes, actions réalisables en 1 tap maximum |
