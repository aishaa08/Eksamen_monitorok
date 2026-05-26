# 🖥️ Eksamen Monitor

Et skoleprosjekt som overvåker en Raspberry Pi i sanntid.
Systemet samler inn CPU-bruk, RAM-bruk og oppetid, og viser
dataene på et web-dashboard laget med Flask.

---

## 📁 Prosjektstruktur

eksamen_monitor/
│
├── app.py
├── README.md
├── cron.log
│
├── scripts/
│   └── monitor.py
│
├── templates/
│   ├── index.html
│   └── navn_ansatte.html
│
└── static/
    ├── style.css
    └── script.js

---

## 🗄️ Database

**Databasenavn:** eksamen_monitor  
**Tabeller:**
- `målinger` — lagrer CPU, RAM og uptime fra Raspberry Pi
- `ansatte` — lagrer navn, rolle og epost til ansatte

---

## ⚙️ Hva systemet gjør

- `monitor.py` samler CPU-bruk, RAM-bruk og oppetid
- Data lagres automatisk i MariaDB via cron job (hvert 20. minutt)
- `app.py` kjører en Flask webserver
- Dashboard viser sanntidsdata fra databasen
- Ansatte-siden viser en oversikt over teamet

---

## 🛠️ Teknologier brukt

- Python 3
- Flask
- MariaDB
- psutil
- HTML / CSS / JavaScript
- Raspberry Pi OS

---

## 👥 Laget av

Aisha  
Skoleprosjekt — 2026 rett før eksamen # Eksamen_monitorok
