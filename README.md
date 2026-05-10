# 📝 Application de Gestion de Notes

## 📌 Description

Cette application web permet à un utilisateur de s’inscrire, se connecter et gérer ses notes personnelles (ajout, modification, suppression).
Chaque note contient un titre, un contenu et un niveau de priorité (low, medium, high).

---

## 🛠️ Technologies utilisées

* Backend : Laravel (API REST + Sanctum)
* Frontend : React (Vite) + Axios
* Base de données : MySQL ou SQLite

---

## ⚙️ Instructions de lancement

### 🔹 1. Télécharger le projet

* Télécharger le projet depuis GitHub (bouton **Code → Download ZIP**)
* Extraire le dossier

---

## 🔧 2. Backend (Laravel)

### 📂 Accéder au dossier backend

```bash id="8jg5m7"
cd notes-app
```

### 📦 Installer les dépendances

```bash id="yjrs7g"
composer install
```

### ⚙️ Configuration

```bash id="7z6z8c"
cp .env.example .env
php artisan key:generate
```

👉 Modifier le fichier `.env` :

```env id="5c69g4"
DB_DATABASE=nom_de_la_base
DB_USERNAME=root
DB_PASSWORD=
```

---

### 🗄️ Migration de la base de données

```bash id="y2i5u7"
php artisan migrate
```

---

### ▶️ Lancer le serveur backend

```bash id="a9q5de"
php artisan serve
```

👉 Backend disponible sur :
http://127.0.0.1:8000

---

## 💻 3. Frontend (React)

### 📂 Accéder au dossier frontend

```bash id="p2rb4c"
cd notes-frontend
```

### 📦 Installer les dépendances

```bash id="2ux0n2"
npm install
```

### ▶️ Lancer le serveur frontend

```bash id="g5u2df"
npm run dev
```

👉 Frontend disponible sur :
http://localhost:5173

---

## 🔐 Authentification

* Authentification via Laravel Sanctum (token)
* Les routes API sont protégées avec `auth:sanctum`

---

## 🚀 Remarque importante

Le projet a été uploadé directement sur GitHub sans utilisation de Git en local.

---

## 👨‍💻 Auteur

Adem Fattouch - Iyed Abaza
