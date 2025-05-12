# Formulaire de Contact Sécurisé

Ce projet crée un formulaire de contact sécurisé en utilisant les principes de **Security by Design**. L'objectif est de protéger les données utilisateurs en respectant les bonnes pratiques de gestion des mots de passe, la protection contre les attaques et la sécurisation de la transmission des données.

## **Prérequis**

Avant de commencer, assurez-vous d'avoir les outils suivants installés sur votre machine :

- **Node.js** (version 14 ou supérieure)
- **OpenSSL** pour générer des certificats SSL locaux (si vous souhaitez utiliser HTTPS)
- **Un éditeur de code** (ex. Visual Studio Code)

## **Installation**

### 1. **Clonez ce repository** :
   Dans votre terminal, clonez ce repository :
   ```bash
   git clone https://github.com/MassinissaBEY/formulaire_securise.git
   cd formulaire_securise 
  ```

### 2. **Installez les dépendances** :
Installez toutes les dépendances nécessaires en exécutant la commande suivante :
Dans votre terminal : ```npm install```

### 3. **Exécution du projet :**
Démarrez le serveur localement, exécutez la commande suivante : node src/server.js

Le serveur sera accessible via https://localhost:3000.

### 4. **Accédez à la page de connexion :
Lors de votre première ouverture du projet dans le navigateur, vous serez redirigé vers une page de connexion. Utilisez les identifiants suivants pour vous connecter :

Email : massi@gmail.com

Mot de passe : motdepasse123


### 5.Rapport de sécurité
Le rapport détaillé avec les tests de sécurité réalisés est disponible dans le dossier rapport_securite/. Vous pouvez également consulter ce rapport pour comprendre les mesures prises pour protéger ce formulaire.


Ce projet a été conçu avec une attention particulière à la sécurité. Voici les tests réalisés pour garantir la protection des données utilisateurs :

Validation du reCAPTCHA côté client et serveur

Protection contre les injections SQL et XSS

Cookies sécurisés avec les flags HttpOnly et Secure

Utilisation de HTTPS pour la transmission des données

Hachage des mots de passe avec bcrypt.



formulaire_securise/
├── config/
│   ├── cert.pem
│   ├── key_no_passphrase.pem
│   └── key.pem
├── logs/
│   ├── access.log
│   └── messages.log
├── public/
│   ├── index.html
│   ├── login.html
│   ├── admin.html
│   └── css/
│       └── style.css
├── data/
│   |
│   │____messages.json
│   | 
│   |____users.json
├── src/
│   |____server.js
│   
│   
│   
└── rapport_securite/
    └── rapport_securite.pdf



