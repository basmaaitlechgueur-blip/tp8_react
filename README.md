# TP 8 – Consommer une API avec Fetch et Axios dans React

## Description

Ce projet React a pour objectif d'apprendre à **consommer une API externe** dans une application React en utilisant deux méthodes différentes :

* **fetch()** (API JavaScript native)
* **Axios** (bibliothèque HTTP populaire)

L'application récupère des données depuis l'API publique **JSONPlaceholder** et les affiche dans l'interface.

---

## Objectifs du TP

Dans ce TP nous avons appris à :

* Comprendre la différence entre **fetch()** et **axios**
* Effectuer des **requêtes HTTP vers une API**
* **Afficher des listes de données** dans React
* Gérer les états :

  * **chargement (loading)**
  * **erreurs (error)**
* Organiser le code avec **plusieurs composants**

---

## Technologies utilisées

* React
* JavaScript (ES6)
* Fetch API
* Axios
* JSONPlaceholder API

---

## Structure du projet

```
tp-api
│
├── node_modules
├── public
├── src
│   ├── App.js
│   ├── FetchData.js
│   ├── AxiosData.js
│   └── index.js
│
├── package.json
└── README.md
```

### Description des fichiers

**App.js**
Composant principal qui affiche les deux composants :

* FetchData
* AxiosData

**FetchData.js**
Composant qui récupère les articles depuis l’API en utilisant **fetch()**.

**AxiosData.js**
Composant qui récupère les utilisateurs depuis l’API en utilisant **axios**.

---

## Installation du projet

1️⃣ Cloner ou créer le projet

```bash
npx create-react-app tp-api
```

2️⃣ Entrer dans le dossier

```bash
cd tp-api
```

3️⃣ Installer Axios

```bash
npm install axios
```

4️⃣ Lancer l'application

```bash
npm start
```

L'application sera disponible sur :

```
http://localhost:3000
```

---

## Fonctionnement de l'application

### 1️⃣ Chargement des articles avec fetch()

Le composant **FetchData** :

* envoie une requête vers :

```
https://jsonplaceholder.typicode.com/posts
```

* récupère les données
* affiche les **5 premiers titres d'articles**

---

### 2️⃣ Chargement des utilisateurs avec Axios

Le composant **AxiosData** :

* envoie une requête vers :

```
https://jsonplaceholder.typicode.com/users
```

* récupère les utilisateurs

* affiche :

* le **nom**

* l'**email**

---

## Gestion des états

Chaque composant gère trois états :

* **loading** → affiche *Chargement en cours...*
* **error** → affiche le message d'erreur
* **data** → affiche les données récupérées

---

## Résultat final

L'application affiche deux sections :

### Articles récupérés avec Fetch

* Liste de titres d'articles

### Utilisateurs récupérés avec Axios

* Liste de noms et emails

---

## Captures d'écran

### Résultat dans le navigateur


<img width="1920" height="952" alt="Screenshot (716)" src="https://github.com/user-attachments/assets/0df154c9-c869-4366-9845-530b76e4ba3b" />
<img width="1920" height="965" alt="Screenshot (717)" src="https://github.com/user-attachments/assets/d4d5d719-a58f-455e-be41-75fae42af951" />

```






## Conclusion

Ce TP montre comment :

* récupérer des données depuis une API
* afficher des listes dans React
* utiliser **fetch()** et **axios**

Axios est souvent préféré car il simplifie la gestion des réponses et des erreurs.

---

**Projet réalisé dans le cadre du TP React – Consommation d’API.**
