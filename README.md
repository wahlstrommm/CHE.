# Restaurang Che

Välkommen till Restaurang Che's officiella hemsida! Detta projekt är byggt med React och TypeScript på frontend och Express med Node.js på backend. Syftet med denna applikation är att ge en modern och användarvänlig plattform för att visa upp restaurangens menyer, evenemang och specialerbjudanden. Personal kan enkelt ladda upp och uppdatera innehåll via en separat inloggningsportal.

## Innehållsförteckning

- [Funktioner](#funktioner)
- [Teknologier](#teknologier)
- [Installation](#installation)
- [Användning](#användning)
- [Projektstruktur](#projektstruktur)
- [API-dokumentation](#api-dokumentation)
- [Bidra](#bidra)
- [Licens](#licens)

## Funktioner

- **Responsiv Design**: Anpassar sig till olika skärmstorlekar.
- **Dynamiska Menyer**: Visa uppdaterade menyer och specialerbjudanden.
- **Evenemangshantering**: Visa kommande evenemang.
- **Backend API**: Hämta och uppdatera data via REST API.
- **Separat Inloggningsportal**: Personal kan ladda upp och uppdatera innehåll via en separat portal.

## Teknologier

- **Frontend**: React, TypeScript
- **Backend**: Node.js, Express
- **Databas**: MongoDB (eller annan valfri databas)
- **Styling**: Styled Components, CSS
- **Autentisering**: JWT (JSON Web Tokens)

## Installation

Följ dessa steg för att köra projektet lokalt:

### Klona Repositoriet

```bash
git clone https://github.com/ditt-användarnamn/restaurang-che.git
cd restaurang-che

Frontend
bash
cd frontend
npm install

Backend
bash
cd ../backend
npm install

Miljövariabler
Skapa en .env-fil i backend-mappen och lägg till följande miljövariabler:
env
PORT=5000
MONGO_URI=din-mongodb-uri
JWT_SECRET=din-hemliga-nyckel

Starta Applikationen
Frontend
bash
cd frontend
npm start

Backend
bash
cd ../backend
npm run dev

Användning
Besök http://localhost:3000 för att se frontend-applikationen.
Backend API är tillgängligt på http://localhost:5000/api.
Projektstruktur
plaintext
restaurang-che/
├── backend/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── .env
│   ├── server.js
│   └── package.json
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── App.tsx
│   │   ├── index.tsx
│   └── package.json
└── README.md

API-dokumentation
Hämta Menyer
http
GET /api/menus

Beskrivning: Hämta alla menyer.
Svar: JSON-array med menyer.
Hämta Evenemang
http
GET /api/events

Beskrivning: Hämta alla evenemang.
Svar: JSON-array med evenemang.
