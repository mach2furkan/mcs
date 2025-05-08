# mcs




# 🛰️ ATHGYS – Tactical Map & Mission Command System

**ATHGYS (Advanced Tactical Hybrid Geolocation & Yielding System)** is a modern, mission-oriented military command dashboard designed to manage units, plan operations, and visualize field intelligence in real time. Built with security and operational awareness in mind, ATHGYS is ideal for defense, disaster response, and field coordination.

---

## 🚀 Features

- 🗺️ **Advanced Interactive Map**  
  Real-time map rendering with unit overlays and contextual menus

- 🧭 **Mission Planning Tools**  
  Assign, track, and manage multiple mission types (recon, logistics, intel, etc.)

- 📡 **WebSocket-Based Communication**  
  Secure, real-time unit and HQ messaging system

- 🧠 **AI-Powered Suggestions** *(experimental)*  
  Tactical pathfinding and threat assessment

- 🔐 **Role-Based User Access Control**  
  Multiple permission levels for operators, commanders, and observers

- ⚠️ **Event & Risk Alerts**  
  Smart warnings based on unit location, weather, and intelligence

- 🧰 **Modular Architecture**  
  Easy to expand with new mission types or integrations

---

## 🛠️ Installation

```bash
# Clone the repository
git clone https://github.com/mach2furkan/mcs.git
cd mcs

# Install dependencies (with legacy peer support)
npm install --legacy-peer-deps

# Start the development server
npm run dev
````

> **Note:** If you encounter a `ERESOLVE` error during `npm install`, use the `--legacy-peer-deps` flag.

---

## 🧩 Project Structure

```
components/
  map-view-enhanced.tsx     # Main map logic and rendering
  unit-panel.tsx            # Dynamic unit interaction panel
utils/
  missionUtils.ts           # Mission type and status handlers
services/
  socket.ts                 # WebSocket connection manager
pages/
  index.tsx                 # Main dashboard page
```

---

## 🐞 Common Error Fix

### ❌ `Unexpected token. Did you mean '{'}'}`

**Cause:**
A stray backslash (`\`) after `item.action();` caused a parsing error.

**Fix:**
Removed the backslash:

```tsx
item.action();
contextMenu.remove();
```

Also, corrected malformed JSX syntax and missing curly braces in `map-view-enhanced.tsx`.

---

## 🎯 Planned Features

* Drone swarm coordination interface
* Offline mode with data sync
* Custom mission templates
* Satellite image overlays
* Performance analytics per mission
* Dark mode / operator theme
* Terrain & weather integration
* Enemy zone marking
* Export to PDF & KML
* Real-time NATO symbol rendering

---

## 📜 License

This project is **private and proprietary**.
All rights reserved © ATHGYS / MCS Team, 2025.

---

## 🤝 Contact

Developed by [Furkan Aşkın](https://github.com/mach2furkan)
For collaboration, contact via GitHub or email.
