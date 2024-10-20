# Cleance

## Introduction

Cleance est une application web permettant aux freelances de pouvoir gérer l’aspect administratif de leur métier. Cleance permet aux freelances de gérer leurs clients en créant des factures / devis liés à leurs clients ainsi que de tenir un cahier de compte. L’idée est de faciliter la gestion des papiers administratifs en centralisant une grande partie dans une application.

## Fonctionnalités

### 2.1 Authentification et gestions des utilisateurs

- Inscription d’un utilisateur avec nom, prénom, email, mot de passe.
- L’utilisateur doit renseigner ensuite :
    - Adresse postale,
    - Site internet (optionnel),
    - Numéro de SIRET,
    - IBAN, BIC, Nom de la Banque
- Connexion d’un utilisateur avec email et mot de passe.
- Réinitialisation du mot de passe.

### 2.2 Gestion des clients

L’utilisateur a la possibilité de créer, modifier et supprimer des clients qui sont propres à lui,
- Lors de la création d’un client, l’utilisateur doit renseigner les informations suivantes :
    - Nom,
    - Email,
    - Téléphone (optionnel),
    - Addresse,
    - Numéro de SIRET

### 2.3 Gestion des factures

L’utilisateur peut créer, modifier et supprimer des factures / devis,
- Lors de la création d’une facture, l’utilisateur doit :
    - Choisir le client à qui il fait la facture,
    - Renseigner la méthode de paiement pour le client (espèce, chèque, virement bancaire),
    - Via un système de répéteur ajouter chaque prestations effectuées au client :
        - Description,
        - Quantité,
        - Prix à l’unité,
- Le numéro de facture et définit automatiquement (YYYY,MM,NUM), les éléments relatifs à l’utilisateur et le client (Nom, adresse…) sont gérés avec une relation en base de donnée.

### 2.4 Gestion des devis

L’utilisateur peut créer, modifier et supprimer des devis,
- Lors de la création d’un devis, l’utilisateur doit :
    - Choisir le client à qui il fait le devis,
    - Renseigner la méthode de paiement pour le client (espèce, chèque, virement bancaire),
    - Via un système de répéteur ajouter chaque prestations effectuées au client :
    - Description,
    - Quantité,
    - Prix à l’unité,
- Le numéro de facture et définit automatiquement (YYYY,MM,NUM), les éléments relatifs à l’utilisateur et le client (Nom, adresse…) sont gérés avec une relation en base de donnée.
- Possibilité de créer directement une facture sur la page du devis quand celui-ci a été accepté.
