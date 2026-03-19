# AGENT.md — afi-machinery-app

## Purpose
A Google Apps Script WebApp for managing machinery maintenance at Advanced Food Industries (AFI). Mobile-first, Arabic-language interface for tracking machine status, maintenance history, and schedules.

## Structure
```
afi-machinery-app/
├── README.md
├── AGENT.md
├── .gitignore
└── src/
    ├── appsscript.json  ← GAS manifest
    ├── env.js           ← Sheet IDs / config
    ├── Backend.js       ← data access layer (Sheets read/write)
    ├── Helpers.js       ← pure utility functions
    ├── Middleware.js    ← server-side routing
    ├── Server.js        ← doGet() / doPost() entry points
    └── index.html       ← SPA shell (dashboard, machine details, schedule)
```

## Key Facts
- **Platform:** Google Apps Script WebApp
- **Data store:** Google Sheets (IDs in `env.js`)
- **Language:** Arabic UI (RTL layout)
- **Features:** Machine status dashboard, maintenance history, maintenance schedule calendar
- **Entry point:** `Server.js` → `doGet()` / `doPost()`

## Development Notes
- All source files live under `src/` — push with clasp from that directory
- No Node/npm at runtime; ES5-compatible GAS code only
- Sheet IDs and secrets live in `env.js` (not committed with real values)
