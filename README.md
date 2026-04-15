<div align="center">
  <img src="https://cdn.evelocore.com/files/Evelocore/projects/evelodb-server/icon.png" width="80" height="80" alt="EveloDB Server" />
  <h1>EveloDB Server</h1>
  <p>The official server implementation for the EveloDB DBMS — featuring a robust API and a modern React-based management panel.</p>
</div>

---

- [📦 Installation](#install)
- [🔄 Update](#update)

---

## ✨ Features

- **TypeScript-first** — Fully migrated to TypeScript across backend and frontend for maximum type safety and developer productivity.
- **Node.js Backend** — Express-based API server with `ts-node` support for fast iteration.
- **React Management Panel** — Vite-powered dashboard with premium dark/light mode for managing databases, collections, and users.
- **EveloDB Shell** — Interactive web terminal powered by Monaco Editor for direct database manipulation.
- **Data Visualization** — Explore collection data in JSON, Table, and List views.

---

## 📋 Prerequisites

- Node.js **v16** or higher
- npm or yarn
- Git

---

<div id="install"></div>

## 📦 Installation

**1. Clone the repository**
```bash
git clone https://github.com/evelocore-release/evelodb-server.git
cd evelodb-server
```

**2. Install dependencies**
```bash
npm install
```

**3. Configure the server**

Edit `config.json` to match your environment:
```json
{
  "panelPort": 7961,
  "serverPort": 7962,
  "origins": [
    "http://localhost:7961"
  ]
}
```

| Field | Description |
|---|---|
| `panelPort` | Port the management panel runs on |
| `serverPort` | Port the API server listens on |
| `origins` | Allowed CORS origins to access the panel |

**4. Start the server**
```bash
npm start
```

---

<div id="update"></div>

## 🔄 Updating

**1. Pull the latest changes**
```bash
git pull origin main
```

**2. Update dependencies**
```bash
npm install
```

**3. Restart the server**
```bash
npm start
```

> **Note:** After major updates, review the changelog for any breaking changes or new environment variables that need to be configured before restarting.

---

## 📖 Component Guidelines

- Use `.ts` for logic-only files.
- Use `.tsx` for React components.
- Interfaces should be defined within the component file or in a dedicated `types/` directory.

---

<div align="center">
  <sub>© 2023 Evelocore Production. All rights reserved.</sub>
</div>