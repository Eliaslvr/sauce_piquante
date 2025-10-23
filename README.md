# 🍽️ Application d'avis gastronomique - Backend et Frontend

## 🎯 Ma mission

Développer le **backend** d'une application d'avis gastronomique permettant aux utilisateurs de créer, modifier, noter et supprimer des sauces.

---

## 🧰 Technologies utilisées

### 🔹 Serveur

* **Node.js**
* **Express.js**

### 🔹 Base de données

* **MongoDB / Mongoose**
* **MongoDB Atlas**

### 🔹 Frontend

* **Angular**
* **Axios**
* **HTML / CSS**

---

## 💡 Le projet

Ce projet consiste à créer une **API REST** sécurisée pour un site de notation de sauces.
Les utilisateurs peuvent :

* S'inscrire / se connecter
* Consulter la liste des sauces
* Créer, modifier et supprimer leurs propres sauces
* Liker ou disliker les sauces d'autres utilisateurs

---

## 📄 Composition du site

### 🔐 Page d'inscription / de connexion

L’utilisateur arrive sur une page sécurisée d’inscription ou de connexion.

* Les mots de passe sont **hachés avec bcrypt** avant d’être enregistrés.
* L’authentification se fait via **JWT (JSON Web Token)**.

### 🏠 Page d’accueil

Une fois authentifié, l’utilisateur accède à la page d’accueil où sont listées toutes les sauces présentes dans la base de données.

### 🌶️ Page descriptive d’une sauce

Chaque sauce dispose d’une page dédiée affichant :

* Son nom, son créateur, sa description
* Son niveau de piquant
* Son nombre de likes et dislikes
* Les boutons pour aimer / ne pas aimer la sauce

### ➕ Page d’ajout de sauce

Un utilisateur connecté peut :

* Ajouter une nouvelle sauce (avec une image)
* Modifier ou supprimer **uniquement** ses propres sauces

---

## 🔒 Sécurité

* **Mots de passe hachés avec bcrypt**
* **Token JWT** pour sécuriser les routes et authentifier les utilisateurs
* **Middleware d’authentification** pour protéger les routes sensibles
* **Gestion sécurisée des fichiers images** avec **Multer**

---

## ⚙️ Installation du projet

### 1️⃣ Cloner le dépôt

```bash
git clone https://github.com/Eliaslvr/sauce_piquante.git
```

### 2️⃣ Installer le backend

```bash
cd backend
npm install
```

### 3️⃣ Créer un fichier `.env`

Dans le dossier `backend`, crée un fichier `.env` avec :

```
PORT=3000
MONGODB_URI=<ton lien MongoDB Atlas>
TOKEN_SECRET=RANDOM_TOKEN_SECRET
```

### 4️⃣ Lancer le backend

```bash
npm start
```

### 5️⃣ Installer le frontend

```bash
cd frontend
npm install
```

### 6️⃣ Lancer le frontend

```bash
npm start
```

Le frontend tourne sur le port `3001` et le backend sur `3000`.

---

## 🥇 Objectif final

Mettre en place une **application complète et sécurisée** permettant à des passionnés de gastronomie de partager, noter et découvrir des sauces du monde entier.
