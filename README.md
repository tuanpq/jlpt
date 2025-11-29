# jlpt
Japanese Language Proficiency Test

# Software Requirements Specification
## Functional Requirements
### Vocabulary list by levels N5 to N1
### Kanji list by levels N5 to N1
### Grammar list by levels N5 to N1
### Sample sentence list by levels N5 to N1

## Non-functional Requirements
### 1 million ccu code
### Zero downtime
### Log collection

# Technical Specification
## Backend
### Language and Framework: Java 21, Spring Boot, PostgreSQL
### Database: PostgreSQL
### Architecture pattern: Microservices
### Project Structure: Package by features
## Frontend
### Language and Framework: Vuejs
### Project Structure: Package by features
## Mobile
### Language and Framework: Flutter
### Project Structure: Package by features

## How to run

Backend (Java 21)
------------------

This project targets Java 21 (latest LTS). Install a JDK 21 distribution and ensure `JAVA_HOME` points to it before building or running the backend services.

On Windows PowerShell, for example:

```powershell
$env:JAVA_HOME = 'C:\Program Files\Java\jdk-21'
```

Then build with Maven from the service folder:

```powershell
cd backend\content-service; mvn -DskipTests package
```

Frontend (Vue)
---------------

The scaffolded Vite + Vue 3 frontend is in `frontend/vue-app`.

```powershell
cd frontend\vue-app
npm install
npm run dev
```

Open http://localhost:5173 (or the address printed by Vite).

Mobile (Flutter)
---------------

The Flutter scaffold is in `mobile/flutter-app`.

Install Flutter SDK and run:

```powershell
cd mobile\flutter-app
flutter pub get
flutter run
```

The mobile scaffold uses a package-by-feature layout and a simple in-memory repository for the Home MVP.
