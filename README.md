# 🚀 Blog Portfolio — Rupesh K R

A full-stack blog portfolio built with **React**, **Firebase**, and **Tailwind CSS** — featuring authentication, real-time blog CRUD, dark/light theme, and a fully responsive design. Live and deployed on Vercel.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-blogportfolio1.vercel.app-brightgreen?style=for-the-badge&logo=vercel)](https://blogportfolio1.vercel.app/home)
[![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react)](https://react.dev/)
[![Firebase](https://img.shields.io/badge/Firebase-10-FFCA28?style=for-the-badge&logo=firebase)](https://firebase.google.com/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-3-06B6D4?style=for-the-badge&logo=tailwindcss)](https://tailwindcss.com/)

---

## 🌐 Live Demo

**[https://blogportfolio1.vercel.app](https://blogportfolio1.vercel.app/home)**

---

## ✨ Features

- 🔐 **Authentication** — Email/password login & signup via Firebase Auth
- 📝 **Blog CRUD** — Create, read, like, and delete blog posts (logged-in users)
- 🔥 **Real-time Database** — Firestore for instant data sync
- 🌗 **Dark / Light Theme** — Persistent theme toggle across all pages
- 📂 **Category Filter** — Filter blogs by Tech, Dev, React, Career, Personal
- ⏱️ **Read Time Estimator** — Auto word count and read time per post
- 📱 **Fully Responsive** — Mobile-first design with Tailwind CSS
- 🛡️ **Protected Routes** — Only authenticated users can create/delete posts
- 📄 **Multi-page SPA** — Home, About, Contact, Blogs, Login, Signup

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend | React 18, React Router v6 |
| Styling | Tailwind CSS 3, PostCSS |
| Auth | Firebase Authentication (Email/Password) |
| Database | Cloud Firestore |
| Deployment | Vercel |
| Backend (optional) | Express.js + Firebase Admin SDK |

---

## 📁 Project Structure

```
portfolio-v2/
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── assets/              # Images and icons
│   │   ├── components/
│   │   │   ├── Home.jsx         # Landing page
│   │   │   ├── Blogs.jsx        # Blog CRUD (Firestore)
│   │   │   ├── About.jsx        # About section
│   │   │   ├── Contact.jsx      # Contact form
│   │   │   ├── Login.jsx        # Firebase login
│   │   │   ├── Signup.jsx       # Firebase signup
│   │   │   └── common/
│   │   │       ├── Navbar.jsx   # Responsive nav + auth state
│   │   │       ├── Footer.jsx
│   │   │       └── PrivateRoute.jsx
│   │   ├── config/
│   │   │   └── firebase.js      # Firebase SDK config
│   │   ├── context/
│   │   │   ├── AuthContext.js   # Global auth state
│   │   │   └── ThemeContext.js  # Dark/light theme state
│   │   ├── App.js
│   │   └── index.js
│   ├── vercel.json              # SPA routing fix for Vercel
│   └── package.json
└── backend/                     # Optional REST API (Express + Firebase Admin)
    ├── index.js
    └── package.json
```

---

## 🚀 Getting Started (Local)

### Prerequisites
- Node.js 18+
- A Firebase project ([Create one here](https://console.firebase.google.com))

### 1. Clone the repo

```bash
git clone https://github.com/your-username/portfolio-v2.git
cd portfolio-v2/frontend
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure Firebase

Edit `src/config/firebase.js` and paste your Firebase project config:

```js
const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_PROJECT.firebaseapp.com",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_PROJECT.appspot.com",
  messagingSenderId: "YOUR_SENDER_ID",
  appId: "YOUR_APP_ID",
};
```

### 4. Run the app

```bash
npm start
# Opens http://localhost:3000
```

---

## ☁️ Deploy to Vercel

1. Push this repo to GitHub
2. Go to [vercel.com](https://vercel.com) → New Project → Import your repo
3. Framework: **Create React App** | Output: `build`
4. Add environment variable: `DISABLE_ESLINT_PLUGIN = true`
5. Click **Deploy** — done!

> The `vercel.json` file handles SPA routing so all routes (`/blogs`, `/login`, etc.) work correctly on direct URL access.

---

## 🔒 Firebase Setup Checklist

- [x] Enable **Email/Password** under Authentication → Sign-in method
- [x] Create **Firestore Database** (start in test mode)
- [x] Add your **Vercel domain** to Authentication → Settings → Authorized domains

---

## 📸 Pages

| Page | Route | Access |
|---|---|---|
| Home | `/home` | Public |
| About | `/about` | Public |
| Contact | `/contact` | Public |
| Blogs | `/blogs` | Public (read) |
| Login | `/login` | Public |
| Signup | `/signup` | Public |
| Write / Delete Blog | `/blogs` | Logged-in users only |

---

## 👨‍💻 Author

**Rupesh K R**
- 💼 Resolution Coordinator @ Walmart Global Tech
- 🎓 B.Tech IT (2024) | CCNA Certified
- 🌱 Transitioning into Full Stack Development (MERN)
- 🔗 [LinkedIn](https://www.linkedin.com/in/your-linkedin) | [Portfolio](https://blogportfolio1.vercel.app)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
