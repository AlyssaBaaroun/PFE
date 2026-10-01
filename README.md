# Cahier des charges
> RushTeam

Application web de gestion des horaires et du personnel développée dans le cadre d'un projet de fin d'études, ciblant les managers, étudiants ainsi que les membres du personnel d’une enseigne de fast-food.

## Sommaire

1. Présentation du projet
2. Contexte de l'application
3. Objectif
4. Personas et parcours utilisateurs
5. Fonctionnalités principales

## Présentation du projet

RushTeam est une application web de gestion des horaires et du personnel, développée dans le cadre d'un projet de fin d'études. Elle cible les managers, les étudiants ainsi que les membres du personnel d'une enseigne de fast-food.

RushTeam centralise ces tâches dans une application accessible depuis un téléphone pour les membres du personnel ainsi que pour les étudiants, les managers peuvent également y avoir accès.

En complément, une version desktop serait développée pour la gestion des horaires / planification de poste pour le manager uniquement.

## Contexte de l'application

Dans la plupart des enseignes de restauration rapide, les horaires sont toujours difficiles d'accès. La plupart sont toujours sur papier et les gens qui y travaillent doivent se déplacer sur place afin de voir quand ils travaillent.

Les différentes informations sont propagées sur plusieurs plateformes, telles que :

* Les horaires
* Les postes attribués à chacun (grill, bornes, take-out, drive…)
* Informations sur certaines procédures à suivre (recette grillman, procédure hygiénique…)
* Changement d'horaire entre membres du personnel
* Discussions entre collègues et managers
* Demande de contrat…

## Objectif

L'objectif est de fournir aux étudiants et aux membres du personnel de l'enseigne de fast-food une application moderne et simple d'utilisation pour gérer au mieux tous les points énoncés ci-dessus.

## Personas et parcours utilisateurs
### Vincent, manager et planificateur d'horaires et des équipes

Il gère une équipe de plus de 40 personnes dont beaucoup d'étudiants. Son objectif est de faire les horaires rapidement et facilement, ainsi que de respecter les disponibilités et contraintes de chaque membre de son équipe.

Il se connecte sur son ordinateur à l'application RushTeam et complète le tableau des horaires en fonction des demandes de contrat reçues dans l'onglet « demande de contrat » et des disponibilités de ses équipiers.

Dans ce tableau, il retrouve :

* Le collaborateur (ex : Alyssa Baaroun)
* Le rôle
* Les jours de la semaine
* Le nombre d'heures à prester par jour et l'horaire planifié
* Les heures contractuelles
* Le total d'heures sur la semaine (parfois un peu plus / un peu moins)
* L'ajout du poste

Une sauvegarde automatique est mise en place et, une fois qu'il a terminé, chaque collaborateur reçoit une notification que le planning a été posté.

### Lisa, étudiante qui souhaite échanger son horaire et contacter son manager pour lui demander la permission

Lisa reçoit son horaire et voit qu'elle a un empêchement le samedi matin alors qu'elle fait un 8-15. Elle voit grâce à l'horaire général que Sabine travaille ce jour-là et fait un 18-1. Elle décide donc d'envoyer un message à Sabine via la messagerie de l'app et lui demande d'échanger son horaire.

Plus tard, après que Sabine a accepté le changement, Lisa envoie ensuite la demande d'échange à Vincent. Une modification sur le linéaire du jour pourra être faite.

### Manon, sous-cheffe qui fait une annonce générale afin que des étudiants reprennent des horaires suite à des personnes qui ne pourront pas assurer leurs horaires

Manon reçoit plusieurs messages d'employés qui ne peuvent pas assurer leurs horaires de la semaine. Elle décide donc de publier une annonce avec les différents horaires à reprendre.

Chaque collaborateur (étudiants / membres) peut se proposer afin de reprendre un ou plusieurs horaires. Des horaires peuvent également ne pas être pris ; dans ce cas, la case reste vide.

### Alice, étudiante qui demande le renouvellement de son contrat étudiant

Le contrat étudiant d'Alice arrive à terme. Elle voit que Vincent a publié une annonce pour les contrats de mars 2027. Elle décide donc d'aller dans l'application et, dans l'onglet « demande de contrat », elle remplit le formulaire de demande.

Dans ce formulaire, on retrouve :

* Le nom et prénom de l'étudiant
* Le nombre d'heures qu'il souhaite faire par semaine
* Les dates de début et de fin de contrat
* Ses disponibilités
* Un moyen d'importer son attestation scolaire ainsi que son student at work
* Le moyen d'ajouter un éventuel commentaire pour le manager qui se chargera de faire les contrats

Alice suit l'état de sa demande dans l'app et reçoit une notification quand son contrat est prêt.

## Fonctionnalités principales

### Partie commune (app mobile)
> Authentification

* Identifiant
* Mot de passe / mot de passe oublié
* Affichage de l'interface selon le rôle

> Horaires

* Notification de quand il est posté
* Vue de son horaire
* Possibilité de voir les horaires des autres
* Consultation de l'horaire hors ligne

> Équipe

* Liste des collaborateurs selon leur rôle
* Fiche d'un collaborateur

> Messagerie

* Conversation privée avec un collègue / manager
* Notification d'un nouveau message

> Annonces

* Réactions aux différentes annonces
* Consultation de différentes annonces

#### Partie collaborateurs (app mobile)
> Demande de contrat

* Formulaire de demande
* Import des différents documents (attestation scolaire, student at work…)
* Feedback de la demande

> Échange d'horaires

* Demande d'échange avec un collègue en privé
* Demande via l'onglet afin que le manager valide le changement (accepté / refusé)

> Horaires à reprendre

* Liste des différents horaires à reprendre (n'importe quel jour de la semaine à venir)

#### Partie sous-chef (app mobile)

* Publication d'annonces
* Publication d'horaires à reprendre

#### Partie chef (app mobile)

* Accepter les changements d'horaires
* Les mêmes fonctionnalités mentionnées au-dessus
* Ajout, modification, suppression d'annonces

#### Partie admin (site web)
> Dashboard

* Demandes en attente
* Demandes de contrat

> Planning

* Affichage du planning de la semaine en cours, mais également des prochaines (non publiées)
* Publication du planning

> Gestion des collaborateurs

* Liste des collaborateurs
* Filtrage selon leur rôle
* Ajout d'un nouveau collaborateur
* Suppression d'un collaborateur (viré ou démission)

> Gestion des différentes demandes

* Validation ou refus des échanges d'horaires
* Liste des demandes de contrat avec consultation des documents
* Acceptation ou refus d'une demande de contrat, avec commentaire si jamais refusé
* Ouverture d'une période de demandes de contrat (annonce)
