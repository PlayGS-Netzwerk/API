# PlayGS Netzwerk API

Die PlayGS Netzwerk API ist eine leistungsstarke RESTful-API, die mit TypeScript, Express, Mongoose, Passport und JSON Web Tokens (JWT) entwickelt wurde. Diese API dient als Backend für das PlayGS Netzwerk und ermöglicht die Verwaltung von Benutzern, Spielen und weiteren Ressourcen.

## Inhaltsverzeichnis

- [Features](#features)
- [Technologien](#technologien)
- [Installation](#installation)
- [Konfiguration](#konfiguration)
- [API-Endpunkte](#api-endpunkte)
- [Nutzung](#nutzung)
- [Beitrag leisten](#beitrag-leisten)
- [Lizenz](#lizenz)

## Features

- Benutzerregistrierung und -anmeldung
- Authentifizierung mit JWT
- CRUD-Operationen für Benutzer und Spiele
- Sicherer Zugriff auf geschützte Routen

## Technologien

- [TypeScript](https://www.typescriptlang.org/)
- [Express](https://expressjs.com/)
- [Mongoose](https://mongoosejs.com/)
- [Passport](http://www.passportjs.org/)
- [jsonwebtoken](https://www.npmjs.com/package/jsonwebtoken)
- [dotenv](https://www.npmjs.com/package/dotenv) (für Umgebungsvariablen)

## Installation

1. Klone das Repository:

   ```bash
   git clone https://github.com/deinbenutzername/playgs-api.git
   cd playgs-api
   ```

2. Installiere die Abhängigkeiten:

   ```bash
   npm install
   ```

3. Erstelle eine `.env`-Datei basierend auf der `.env.example`-Datei und konfiguriere deine Umgebungsvariablen.

## Konfiguration

- Stelle sicher, dass du MongoDB installiert hast oder verwende eine gehostete MongoDB-Lösung (z. B. MongoDB Atlas).
- Konfiguriere die Umgebungsvariablen in deiner `.env`-Datei:
  
  ```
  PORT=3000
  MONGODB_URI=mongodb://localhost:27017/playgs
  JWT_SECRET=dein_geheimes_jwt_schlüssel
  ```

## API-Endpunkte

Hier sind einige der grundlegenden API-Endpunkte:

### Benutzer

- `POST /api/auth/register` - Registriere einen neuen Benutzer
- `POST /api/auth/login` - Melde einen Benutzer an

### Spiele

- `GET /api/games` - Liste aller Spiele abrufen
- `POST /api/games` - Neues Spiel erstellen
- `GET /api/games/:id` - Spieldetails abrufen
- `PUT /api/games/:id` - Spiel aktualisieren
- `DELETE /api/games/:id` - Spiel löschen

## Nutzung

Starte den Server:

```bash
npm run dev
```

Der Server läuft standardmäßig auf `http://localhost:3000`.

## Beitrag leisten

Beiträge sind willkommen! Bitte öffne ein Issue oder erstelle einen Pull Request, um Ideen oder Verbesserungen vorzuschlagen.

## Lizenz

Dieses Projekt steht unter der MIT-Lizenz. Siehe die [LICENSE](LICENSE)-Datei für weitere Informationen.