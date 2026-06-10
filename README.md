<div align="center">

# 📝 Syntecxhub Notes App

**A modern, responsive Notes Application built with React + Vite**

[![React](https://img.shields.io/badge/React-18.x-61DAFB?style=for-the-badge&logo=react&logoColor=white)](https://reactjs.org/)
[![Vite](https://img.shields.io/badge/Vite-5.x-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev/)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Netlify](https://img.shields.io/badge/Netlify-Live-00C7B7?style=for-the-badge&logo=netlify&logoColor=white)](https://syntecxhub-notes-app.netlify.app/)
[![License](https://img.shields.io/badge/License-Educational-orange?style=for-the-badge)](#-license)

<br/>

[🌐 Live Demo](https://syntecxhub-notes-app.netlify.app/) &nbsp;·&nbsp; [📂 Repository](https://github.com/ItsRiku237/Syntecxhub_Notes_App) &nbsp;·&nbsp; [🐛 Report Bug](https://github.com/ItsRiku237/Syntecxhub_Notes_App/issues) &nbsp;·&nbsp; [✨ Request Feature](https://github.com/ItsRiku237/Syntecxhub_Notes_App/issues)

</div>

---

## 🖼 App Screenshots

### 🏠 Home Page
![Home Page](screenshots/Home_page.png)

### 🧭 Sidebar Navigation with Home
![Sidebar Navigation](screenshots/preview.png)

### ➕ Add Note
![Add Note](screenshots/Add_note.png)

### 🎨 Drawing Notes
![Drawing Notes](screenshots/Drawing_notes.png)

### 🌙 Dark Mode
![Dark Mode](screenshots/Dark_mode.png)

### 📂 Sidebar with Footer
![Sidebar with Footer](screenshots/Sidebar_with_Fotter.png)

---

## 📖 Table of Contents

- [About the Project](#-about-the-project)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [Components Overview](#-components-overview)
- [Getting Started](#-getting-started)
- [Usage](#-usage)
- [Future Improvements](#-future-improvements)
- [Developer](#-developer)
- [Acknowledgements](#-acknowledgements)

---

## 🎯 About the Project

Syntecxhub Notes App is a feature-rich, responsive web application for creating, organizing, and managing notes right in your browser. Built during the **Syntecxhub Web Development Internship**, it demonstrates real-world React development — from component architecture to local state persistence.

The app supports **multiple note types** (Standard, Checklist, Image, Drawing), **category organization**, **pinned notes**, **dark mode**, and a **search interface** — all without any backend.

> 💾 Notes are saved using **localStorage** — they persist across page refreshes but are stored per browser/device.

---

## ✨ Features

| Feature | Description |
|--------|-------------|
| ➕ Create Notes | Quick-draft input with `+ New Note` button |
| ✏️ Edit Notes | Inline editing for any existing note |
| 🗑️ Delete & Bin | Delete notes with a recoverable Bin section |
| 📌 Pin Notes | Pin important notes to keep them at the top |
| 📋 Note Types | Standard Note, Checklist List, Image Note, Drawing Canvas |
| 🏷️ Categories | Organize by General, Work, Personal, Ideas, Learning, Guides |
| 🗃️ Archive | Archive notes to declutter without deleting |
| 🌙 Dark Mode | One-click dark/light theme toggle |
| 🔍 Search | Search bar to quickly find notes |
| 📱 Responsive | Works on desktop, tablet, and mobile |
| ⚡ Fast | Vite-powered build for near-instant performance |

---

## 🛠 Tech Stack

| Category        | Technology           |
|-----------------|----------------------|
| Frontend        | React.js (JSX)       |
| Build Tool      | Vite                 |
| Language        | JavaScript (ES6+)    |
| Styling         | CSS3 (per-component) |
| Icons           | Lucide React         |
| Storage         | Browser localStorage |
| Version Control | Git & GitHub         |
| Deployment      | Netlify              |

---

## 📁 Project Structure



```text
Syntecxhub_Notes_App/
│
├── public/                        # Static public assets
│
├── src/                           # Main source code
│   │
│   ├── assets/                    # Images, icons, static resources
│   │
│   ├── components/                # All reusable UI components
│   │   ├── Header.jsx             # Top navigation bar + search
│   │   ├── Header.css             # Header styles
│   │   ├── Sidebar.jsx            # Left sidebar (categories, filters)
│   │   ├── Sidebar.css            # Sidebar styles
│   │   ├── NoteCard.jsx           # Individual note display card
│   │   ├── NoteCard.css           # NoteCard styles
│   │   ├── NoteForm.jsx           # Create / Edit note form
│   │   ├── NoteForm.css           # NoteForm styles
│   │   ├── NotesGrid.jsx          # Grid layout for all note cards
│   │   └── NotesGrid.css          # NotesGrid styles
│   │
│   ├── App.jsx                    # Root component — state & logic
│   ├── index.css                  # Global styles
│   └── main.jsx                   # React DOM entry point
│
├── screenshots/                   # App screenshots for README
│   ├── Home_page.png
│   ├── preview.png
│   ├── Add_note.png
│   ├── Drawing_notes.png
│   ├── Dark_mode.png
│   └── Sidebar_with_Fotter.png
│
├── .gitignore                     # Files excluded from Git
├── eslint.config.js               # ESLint configuration
├── index.html                     # HTML shell (Vite entry)
├── package.json                   # Project metadata & dependencies
├── package-lock.json              # Locked dependency tree
├── vite.config.js                 # Vite build configuration
└── README.md                      # Project documentation
```




---

## 🧩 Components Overview

| Component | Role |
|-----------|------|
| `App.jsx` | Root component; manages global state (notes, dark mode, active category) |
| `Header.jsx` | Top bar with app title, search input, and `+ New Note` button |
| `Sidebar.jsx` | Left panel with All Notes, Pinned, Photo Notes, Archived, Bin, and Categories |
| `NotesGrid.jsx` | Renders the responsive 3-column card grid filtered by active category |
| `NoteCard.jsx` | Individual ngirm to create or edit a note; includes note type selector (Standard, Checklist, Image, Drawing) |

---

## 🚀 Getting Started

### Prerequisites

Ensure the following are installed:

- [Node.js](https://nodejs.org/) — v16 or higher
- [Git](https://git-scm.com/)
- npm — comes bundled with Node.js

### Installation

**1. Clone the repository**
```bash
git clone https://github.com/ItsRiku237/Syntecxhub_Notes_App.git
```

**2. Navigate into the project**
```bash
cd Syntecxhub_Notes_App
```

**3. Install dependencies**
```bash
npm install
```

**4. Start the development server**
```bash
npm run dev
```

App runs at → `http://localhost:5173`

### Build for Production

```bash
npm run build
```

**Preview the production build locally:**
```bash
npm run preview
```

---

## 💡 Usage

1. Open the app or visit the [live demo](https://syntecxhub-notes-app.netlify.app/)
2. Click **`+ New Note`** or type in the quick draft bar and press **Add Note**
3. Choose a note type: **Standard Note**, **Checklist List**, **Image Note**, or **Drawing Canvas**
4. Use the **Sidebar** to filter by category or view Pinned / Archived / Bin
5. Use the **Search bar** to find notes by keyword
6. On each note card:
   - 📌 **Pin** — keep it at the top
   - 🗃️ **Archive** — hide without deleting
   - ✏️ **Edit** — modify content
   - 🗑️ **Delete** — move to Bin
7. Toggle **Dark Theme Mode** from the bottom-left of the sidebar

---

## 📈 Future Improvements

- [ ] 🔐 User Authentication (login/signup)
- [ ] ☁️ Cloud sync — Firebase or Supabase backend
- [ ] 📝 Rich Text Editor (bold, italic, bullet lists)
- [ ] 🖼️ Full Image Note upload support
- [ ] 🎨 Drawing Canvas with color palette
- [ ] 🔔 Reminders & due dates on notes
- [ ] 📤 Export notes as PDF or `.txt`
- [ ] 🏷️ Custom tag creation

---

## 👨‍💻 Developer

<div align="center">

**Riku Sahu**

B.Tech Computer Science & Engineering — GCE Kalahandi
Web Development Intern @ Syntecxhub

[![GitHub](https://img.shields.io/badge/GitHub-ItsRiku237-181717?style=flat-square&logo=github)](https://github.com/ItsRiku237)

</div>

---

## 🙏 Acknowledgements

- [Syntecxhub](https://syntecxhub.com) — for the hands-on internship program
- [React Docs](https://reactjs.org/docs) — component & state reference
- [Vite Docs](https://vitejs.dev/guide/) — build tool documentation
- [Lucide React](https://lucide.dev/) — open-source icon library
- [Netlify](https://netlify.com) — free deployment platform

---

## 📄 License

Developed for **educational and internship purposes** under the Syntecxhub Web Development Internship Program.

---

<div align="center">

Made with ❤️ by **Riku Sahu** &nbsp;|&nbsp; Syntecxhub Internship 2025–26

</div>