# AFI Machinery Maintenance System

A Google Apps Script WebApp for tracking and managing machinery maintenance at Advanced Food Industries (AFI). Mobile-first, Arabic-language interface designed for technicians on the production floor.

![Google Apps Script](https://img.shields.io/badge/Google%20Apps%20Script-4285F4?style=flat&logo=google&logoColor=white)
![Platform](https://img.shields.io/badge/Platform-WebApp-blue)
![Language](https://img.shields.io/badge/UI%20Language-Arabic%20(RTL)-orange)
![Status](https://img.shields.io/badge/Status-Production-green)

---

## About AFI

شركة الصناعات الغذائية المتطورة (Advanced Food Industries) is a food manufacturing enterprise specialising in meat processing, rice packaging, and maamoul production, based in Egypt. This system covers maintenance operations across all production departments.

---

## Features

- Machine management and status tracking (Operational · Maintenance · Breakdown)
- Maintenance scheduling and monitoring
- Real-time status updates and search/filter
- Performance analytics — MTBF, MTTR, uptime percentages
- Document management for equipment manuals and compliance certificates
- Arabic language UI with full RTL layout
- Mobile-first, touch-optimised for production floor use

---

## Tech Stack

| Layer    | Technology                          |
|----------|-------------------------------------|
| Platform | Google Apps Script                  |
| UI       | HTML5, CSS3, Vanilla JavaScript     |
| Database | Google Sheets (Sheets API v4)       |
| Library  | AFI Controller Library (CRUD ops)   |
| Deploy   | clasp CLI                           |

---

## Project Structure

```
afi-machinery-app/
├── README.md
├── AGENT.md
├── .gitignore
└── src/
    ├── appsscript.json  # GAS manifest
    ├── env.js           # Sheet IDs and config
    ├── Backend.js       # Data access layer (Sheets read/write)
    ├── Helpers.js       # Pure utility functions
    ├── Middleware.js    # Server-side routing
    ├── Server.js        # doGet() / doPost() entry points
    └── index.html       # SPA shell (dashboard, machine details, schedule)
```

---

## Getting Started

### Prerequisites

- A Google account with Google Apps Script access
- [clasp](https://github.com/google/clasp) installed globally

```bash
npm install -g @google/clasp
clasp login
```

### Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/mohamedallam13/afi-machinery-app.git
   cd afi-machinery-app
   ```

2. Link to your Apps Script project:
   ```bash
   clasp create --type webapp --title "AFI Machinery" --rootDir src
   ```

3. Push source files:
   ```bash
   clasp push
   ```

4. Set Sheet IDs and any config values in `env.js`.

---

## Deployment

Deployed as a Google Apps Script Web App:

- **Execute as**: User deploying the web app
- **Who has access**: Anyone (or restrict to organisation)
- **Timezone**: Africa/Cairo

To redeploy after changes:

1. In the Apps Script editor, go to **Deploy > Manage deployments**
2. Create a new version and update the active deployment

---

## Author

**Mohamed Allam** — [GitHub](https://github.com/mohamedallam13) · [Email](mailto:mohamedallam.tu@gmail.com)
