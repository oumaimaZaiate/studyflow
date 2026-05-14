# 🎓 StudyFlow — Student Productivity Platform

A complete Laravel MVP for students: Pomodoro, Notes, Flashcards, Streaks, Gamification, and more.

---

## ⚙️ Requirements

- PHP 8.2+
- Composer
- XAMPP (Apache + MySQL)
- Node.js + npm

---

## 🚀 Installation (XAMPP)

### Step 1 — Install Laravel & dependencies

```bash
# In your XAMPP htdocs folder (or any folder served by Apache):
composer create-project laravel/laravel studyflow
cd studyflow

# Install Breeze (auth scaffolding)
composer require laravel/breeze --dev
php artisan breeze:install blade
npm install && npm run build
```

### Step 2 — Copy all provided files into the project

Copy each file from this archive into the corresponding path inside `studyflow/`.

### Step 3 — Configure .env

```
APP_NAME=StudyFlow
APP_URL=http://localhost/studyflow/public

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=studyflow
DB_USERNAME=root
DB_PASSWORD=
```

### Step 4 — Create database

Open phpMyAdmin → create a database named `studyflow`.

### Step 5 — Run migrations & seeders

```bash
php artisan migrate --seed
php artisan storage:link
```

### Step 6 — Run the app

**Option A — Laravel dev server:**
```bash
php artisan serve
# Visit: http://127.0.0.1:8000
```

**Option B — XAMPP Apache:**
Set `APP_URL=http://localhost/studyflow/public` in `.env`  
Visit: `http://localhost/studyflow/public`

---

## 🗂️ Features

| Feature | Route |
|---|---|
| Dashboard | `/dashboard` |
| Study Tasks | `/tasks` |
| Notes | `/notes` |
| Pomodoro | `/pomodoro` |
| Flashcards | `/flashcards` |
| Exams | `/exams` |
| Profile | `/profile` |
