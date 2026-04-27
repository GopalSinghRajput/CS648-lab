# 🧪 Lab 13: React Integration with Express

[![License: ISC](https://img.shields.io/badge/License-ISC-blue.svg)](https://opensource.org/licenses/ISC)
[![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB)](https://reactjs.org/)
[![Express](https://img.shields.io/badge/Express.js-000000?style=flat&logo=express&logoColor=white)](https://expressjs.com/)
[![Babel](https://img.shields.io/badge/Babel-F9DC3E?style=flat&logo=babel&logoColor=black)](https://babeljs.io/)

A focused laboratory exercise demonstrating the integration of a **React** frontend with an **Express.js** backend, featuring real-time JSX compilation and static file serving.

---

## 🛠️ Tech Stack

| Technology | Purpose |
| :--- | :--- |
| **React** | Frontend UI (Loaded via CDN) |
| **Express** | Backend Server & Static Hosting |
| **Babel CLI** | Real-time JSX to JS Compilation |
| **Nodemon** | Development Server Auto-restart |

---

## 🚀 Getting Started

### Prerequisites

Ensure you have [Node.js](https://nodejs.org/) installed on your machine.

### Installation

1. Navigate to the project directory:
   ```bash
   cd lab-13
   ```
2. Install the necessary dependencies:
   ```bash
   npm install
   ```

---

## 💻 Usage

To run the application, you need to open **two separate terminal windows**:

### Step 1: Start Babel Watcher
In the first terminal, run the watcher to compile JSX files in `src/` to `public/` in real-time:
```bash
npm run watch
```

### Step 2: Start the Express Server
In the second terminal, start the backend server:
```bash
npm start
```

### Step 3: Access the App
Once both services are running, open your browser and navigate to:
👉 **[http://localhost:3000](http://localhost:3000)**

---

## 📂 Project Structure

```text
lab-13/
├── public/          # Compiled JavaScript and static assets
├── src/             # Source React components (JSX)
├── app.js           # Express server configuration
├── package.json     # Project dependencies and scripts
└── README.MD        # Documentation
```

---

## 💡 Key Notes

> [!IMPORTANT]
> **Why a Local Server?**
> Browsers block loading local files via the `file://` protocol due to **CORS (Cross-Origin Resource Sharing)** restrictions. An Express server is required to serve these files over `http://`.

> [!TIP]
> - **CDN Loading:** This lab loads React and ReactDOM via CDN links in the HTML for simplicity.
> - **JSX Compilation:** The `npm run watch` command uses Babel CLI to ensure your React code is readable by the browser.

---

<p align="center">
  Developed for CS648 Laboratory Exercise
</p>