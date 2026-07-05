# Business rules

## 1. Gestion des comptes

### 1.1 Unicité de l’email

Un email ne peut être associé qu'à un seul compte.

### 1.2 Un compte peut être client et restaurateur

Un compte peut tout à fait avoir un restaurant et être client d'autres établissements, par contre il ne bénéficiera des fonctionnalités restaurateur que s’il souscrit un abonnement.

### 1.3 Authentification obligatoire

Un restaurateur doit être connecté pour accéder à son espace.

### 1.4 Accès conditionné à un abonnement

Les fonctionnalités restaurateur ne sont accessibles qu’après souscription d’un abonnement actif.

### 1.5 Modification de l’email

La modification de l’email nécessite une vérification via un code à 6 chiffres envoyé à la nouvelle adresse. L’ancien email reste actif jusqu'à validation.

### 1.6 Suppression du compte

La suppression d’un compte est définitive après un délai de 30 jours suivant la demande. Les informations du restaurant sont dépubliées immédiatement. L’utilisateur peut annuler sa demande pendant ce délai.

## 2. Gestion des rôles

### 2.1 Trois rôles distincts

La plateforme définit trois rôles par défaut : Administrateur, Serveur, Invité.

### 2.2 Droits de l’administrateur

Par défaut, l’administrateur peut gérer le menu, les tables, les rôles des utilisateurs et consulter les statistiques.

### 2.3 Droits du serveur

Par défaut, le serveur peut consulter les commandes en cours et mettre à jour leurs statuts.

### 2.4 Droits de l’invité

L’invité peut uniquement consulter le menu et passer commande sur place.

### 2.5 Droits du client connecté

Le client connecté a les mêmes droits que l’invité, mais peut également consulter ses données personnelles, ses historiques de restaurants et commandes, ses lieux recherchés, ses favoris ainsi que certaines statistiques le concernant.

### 2.6 Modification des droits

L’administrateur peut modifier les droits associés à chaque rôle.

## 3. Profil utilisateur

### 3.1 Préférences linguistiques

Un utilisateur peut définir une langue préférée parmi celles disponibles sur la plateforme. Cette préférence s’applique à l’ensemble de l’interface à chaque connexion.

### 3.2 Gestion des favoris

Un client connecté peut ajouter ou retirer des restaurants de sa liste de favoris. Un favori redirige vers la page vitrine.

### 3.3 Gestion des allergènes personnels

Un client connecté peut renseigner ses allergènes. Les plats contenant ces allergènes sont signalés visuellement lors de la consultation du menu.

## 4. Gestion du restaurant

### 4.1 Rattachement obligatoire

Un restaurant est obligatoirement lié à un compte restaurateur actif.

### 4.2 Informations minimales requises 

Un restaurant doit contenir au minimum un nom, une adresse et au moins un horaire d’ouverture pour être publié.

### 4.3 Accès restreint par rôle

La gestion du restaurant est limitée aux utilisateurs autorisés selon leur rôle défini.

### 4.4 Actualités et événements

Un restaurant peut publier des actualités avec un titre, une description et une date. Une actualité expirée peut être archivée ou supprimée

## 5. Gestion des cartes

### 5.1 Structure hiérarchique

Une carte contient des menus et des plats. Un menu contient des plats. Un plat est l'élément de base, il peut appartenir à une carte directement ou à un menu.

### 5.2 Rattachement obligatoire

Une carte est obligatoirement rattachée à un restaurant. Un menu est obligatoirement rattaché à une carte. Un plat est obligatoirement rattaché à une carte ou un menu.

### 5.3 Informations minimales requises

Une carte doit contenir au minimum un nom et au moins un plat ou un menu pour être publiée.

Un menu doit contenir au minimum un nom et au moins un plat.

Un plat doit contenir au minimum un nom et un prix strictement supérieur à 0.

### 5.4 Mise à jour

Toute modification d’une carte, d’un menu ou d’un plat est immédiatement visible par les clients via QR code une fois publiée.

## 6.Gestion des tables

### 6.1 Rattachement obligatoire

Une table est obligatoirement rattachée à une salle, qui elle même est rattachée à un restaurant.

### 6.2 QR code par table

Chaque table possède un QR code unique qui lui est rattaché.

### 6.3 Fusion de tables

Deux tables peuvent être fusionnées pendant un service actif. Les commandes associées sont regroupées automatiquement.

## 7. Gestion des QR codes

### 7.1 QR code global unique

Chaque restaurant possède un QR code global unique redirigeant vers sa page vitrine.

### 7.2 QR code par table unique

Chaque table possède un QR code unique rattaché au restaurant et permettant la commande sur place.

### 7.3 QR code actif

Un QR code ne redirige que vers un menu ou une vitrine existants et publiés.

## 8. Gestion du service

### 8.1 Ouverture et fermeture du service

Le service peut être ouvert et fermé manuellement par le staff autorisé. Lorsque le service est fermé, les tables et la prise de commande ne sont plus accessibles aux clients.

### 8.2 Ouverture automatique

Le service peut être configuré pour s’ouvrir automatiquement selon des horaires définis dans les paramètres du restaurant.

### 8.3 Carte du service

Avant ou pendant un service, le restaurateur peut sélectionner ou modifier la carte active. Les modifications peuvent être sauvegardées comme nouvelle carte ou appliquées uniquement pour ce service.

### 8.4 Code d’accès salle

Un code d’accès peut être activé sur le plan de table pour éviter les commandes frauduleuses à l’intérieur et à l’extérieur du restaurant.

### 8.5 Historique de service

L’historique de chaque service est accessible à l’administrateur (modifications d’articles, de carte et de plan de table sont tracées avec l’auteur et l’horodatage)

## 9. Gestion des commandes

### 9.1 Rattachement obligatoire

Une commande est obligatoirement liée à un restaurant et associée à une table.

### 9.2 Commande non vide

Une commande doit contenir au moins un plat.

### 9.3 Confirmation obligatoire

Une commande doit être validée par le client avant d'être transmise en cuisine.

### 9.4 Statuts de commande

Une commande suit les statuts suivants dans l’ordre : Envoyée → En préparation → Prête → Servie.

### 9.5 Mise à jour du statut

Le staff autorisé peut modifier le statut d’une commande. Chaque changement de statut notifie les parties concernées.

### 9.6 Commande inactive hors service

Aucune commande ne peut être passée lorsque le service est fermé.

## 10. Affichage client

### 10.1 Carte visible uniquement si pubiée

Une carte doit être active et publiée pour être affichée au client via QR code.

### 10.2 Accessibilité mobile

Le menu doit être accessible et lisible depuis un smartphone sans installation d’application.

### 10.3 Suivi de commande

Le client peut suivre le statut de sa commande en cours depuis son téléphone pendant la sessions.

### 10.4 Traduction du contenu

Le contenu affiché au client s’adapte à ses préférences linguistiques. Si le contenu du restaurant n’est pas disponible dans la langue choisie, la langue par défaut du restaurant s’affiche.

### 10.5 Signalement des allergènes

Les plats contenant des allergènes renseignés dans le profil du client connecté sont signalés visuellement dans le menu.

### 10.6 Historique des récapitulatifs

Le client connecté peut consulter l’historique de ses récapitulatifs de commandes. Cette fonctionnalité n’est pas accessible à un client non connecté.

### 10.7 Recherche de restaurant

Un restaurant publié est accessible via la recherche par nom et par lieu.

## 11. Statistiques

### 11.1 Données basées sur les commandes 

Les statistiques sont calculées à partir des commandes et scans QR  enregistrés sur la plateforme.

### 11.2 Accès restreint

Les statistiques qui concernent l'établissement et les commandes sont accessibles uniquement par l’administrateur du restaurant.

### 11.3 Données non personnelles

Les statistiques affichées sont agrégées et n’exposent aucune donnée personnelle identifiable.

### 11.4 Granularité temporelle

Les statistiques sont disponibles par jour et par service, permettant une analyse à la fois macro et opérationnelle.
