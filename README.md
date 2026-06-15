# MonksDocTracker
Tracking system to track document uploads coming in from members

<div align="center">

# 📋 MonksDocTracker

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=4F8EF7&center=true&vCenter=true&width=500&lines=Document+Submission+Tracker;Real-time+sync+across+admins;11+Groups+%C3%97+7+Members+%C3%97+8+Docs" alt="Typing SVG" />

<br/>

![Status](https://img.shields.io/badge/status-live-2dce89?style=for-the-badge&logo=firebase)
![Built with](https://img.shields.io/badge/built%20with-Firebase-FF6F00?style=for-the-badge&logo=firebase)
![Hosted on](https://img.shields.io/badge/hosted%20on-GitHub%20Pages-181717?style=for-the-badge&logo=github)
![Plan](https://img.shields.io/badge/Firebase%20plan-Spark%20(free)-4F8EF7?style=for-the-badge)

<br/>

**A lightweight real-time document submission tracker for team managers.**
Mark documents as received, track progress per player, per group, and overall — synced instantly between admins.

<br/>

🔗 **[Live App →](https://fantasma-27.github.io/MonksDocTracker/)**

</div>

---

## ✨ Features

- 🔐 **Admin login** — only authorised users can access the tracker
- ⚡ **Real-time sync** — both admins see changes instantly, no refresh needed
- 📊 **Three-level progress bars** — per player, per group, and overall
- 📝 **8 documents tracked per member** — Cert 1–5, Photo, ID, Form
- 👥 **11 groups × 7 members** — 616 documents total
- 🌍 **Works anywhere** — Mauritius, Kenya, anywhere with a browser
- 📱 **Mobile friendly** — works on phone and desktop

---

## 🏗️ Structure

```
MonksDocTracker/
├── index.html      # Entire app (HTML + CSS + JS)
└── README.md       # This file
```

> `config.js` lives locally only and is listed in `.gitignore` — your Firebase credentials never touch GitHub.

---

## 🔒 Security

| Layer | What it does |
|---|---|
| Firebase Auth | Only signed-in admins can open the app |
| Firestore Rules | Only authenticated users can read/write data |
| API Key restriction | Key only works from the GitHub Pages domain |

---

## 🛠️ Tech stack

| Tool | Purpose |
|---|---|
| HTML / CSS / JS | Frontend — no frameworks |
| Firebase Auth | Admin login |
| Cloud Firestore | Real-time database |
| GitHub Pages | Free hosting |

---

## 👥 Admins

| Name | Location |
|---|---|
| Admin 1 | 🇲🇺 Mauritius |
| Admin 2 | 🇰🇪 Kenya |

---

<div align="center">

Built for the Monks rugby programme 🏉

</div>
