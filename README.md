<div align="center">

# 🏉 CUEA Monks Off Pitch RTP

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=20&pause=1000&color=CC0000&center=true&vCenter=true&width=550&lines=Document+Submission+Tracker;Real-time+sync+across+admins;Dynamic+Pods+%C2%B7+Player+Management;Search+%C2%B7+Progress+%C2%B7+Rugby+Ball+Gauge" alt="Typing SVG" />

<br/>

![Status](https://img.shields.io/badge/status-live-2dce89?style=for-the-badge)
![Built with](https://img.shields.io/badge/built%20with-Firebase-FF6F00?style=for-the-badge&logo=firebase)
![Hosted on](https://img.shields.io/badge/hosted%20on-GitHub%20Pages-181717?style=for-the-badge&logo=github)
![Plan](https://img.shields.io/badge/Firebase-Spark%20(free)-CC0000?style=for-the-badge)

<br/>

**Internal admin tool for tracking player document submissions across pods.**
Two admins — one in Mauritius 🇲🇺, one in Kenya 🇰🇪 — see the same data in real time.

<br/>

🔗 **[Live App →](https://fantasma-27.github.io/MonksDocTracker/)**

</div>

---

## ✨ Features

- 🔐 **Admin login** — Firebase email/password auth, no public access
- ⚡ **Real-time sync** — both admins see every change instantly
- 🏉 **Rugby ball gauge** — overall progress fills up like a real ball being coloured in
- 🔍 **Player search** — find any player instantly, click to jump to their row
- 📦 **Dynamic pods** — add, rename, or remove pods from the UI
- 👤 **Player management** — add, rename, or remove players per pod
- 📊 **Striped progress bar** — 11 segments per player, one per document, turn green as received
- 📋 **11 documents tracked per player:**
  - Passport Photo
  - National ID / Birth Certificate
  - Player Profile Form
  - Code of Conduct / Agreement
  - Rugby Ready *(World Rugby Passport)*
  - Laws of the Game *(World Rugby Passport)*
  - First Aid in Rugby *(World Rugby Passport)*
  - Concussion Management *(World Rugby Passport)*
  - Keep Rugby Clean *(World Rugby Passport)*
  - Introduction to Coaching *(World Rugby Passport)*
  - Introduction to Officiating *(World Rugby Passport)*
- 🌍 **Works anywhere** — mobile and desktop friendly
- 🔒 **Player names are private** — stored in Firestore behind auth, not in source code

---

## 🏗️ Structure

```
MonksDocTracker/
├── index.html        # Entire app — HTML, CSS, JS in one file
├── monks-logo.png    # Club crest shown on login and header
└── README.md         # This file
```

> Firebase config is embedded in `index.html` with API key restricted to this domain only.
> Player names and progress data live in Firestore — never exposed in the repository.

---

## 🔒 Security

| Layer | Protection |
|---|---|
| Firebase Auth | Only signed-in admins can open the app |
| Firestore Rules | `allow read, write: if request.auth != null` |
| API Key restriction | Key locked to `fantasma-27.github.io` domain only |
| Player data | Names and progress stored in Firestore, not in source code |

---

## 🛠️ Tech stack

| Tool | Purpose |
|---|---|
| HTML / CSS / JS | Frontend — zero frameworks, one file |
| Firebase Auth | Admin login (email + password) |
| Cloud Firestore | Real-time database — pods, players, progress |
| GitHub Pages | Free static hosting |

---

## 👥 Admins

| Role | Location |
|---|---|
| Admin 1 | 🇲🇺 Mauritius |
| Admin 2 | 🇰🇪 Kenya |

---

## 📱 How to use

1. Open the app and sign in with your admin credentials
2. Click **+ Add Pod** to create a pod
3. Open a pod and type a player name → **+ Add** to register them
4. As documents arrive by email, open the player's row and click each document button to mark it received
5. Use the **search bar** to find any player instantly across all pods
6. Progress syncs in real time — no refresh needed

---

<div align="center">

Built for the CUEA Monks Rugby Club 🏉 by <a href="https://fantasma-27.github.io">Fantasma</a>

</div>
