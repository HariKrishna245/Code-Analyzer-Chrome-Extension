# 🚀 CodeScope – Chrome Code Analyzer Extension

<p align="center">
  <img src="https://raw.githubusercontent.com/placeholder/codescope-banner.png" alt="CodeScope Banner" width="100%">
</p>

> 📝 *Replace the banner URL above with your own image — I’ll generate one if you want!*

---

![Chrome](https://img.shields.io/badge/Chrome-Extension-blue)
![TypeScript](https://img.shields.io/badge/TypeScript-Ready-blue)
![React](https://img.shields.io/badge/React-18-61DAFB?logo=react&logoColor=white)
![Webpack](https://img.shields.io/badge/Bundled%20With-Webpack-8DD6F9?logo=webpack&logoColor=white)
![Status](https://img.shields.io/badge/Build-Stable-brightgreen)
![Platform](https://img.shields.io/badge/Platform-Web-lightgrey)

---

## 🎥 Demo Preview

<p align="center">
  <img src="https://raw.githubusercontent.com/placeholder/codescope-demo.gif" width="65%" alt="Demo GIF">
</p>

> 📝 *Drop your demo recording as `demo.gif` into your repo, and replace the link above.*

---

## 📌 Overview

**CodeScope** is a lightweight Chrome extension designed to help developers quickly understand and evaluate source code inside the browser.  
It provides insights into:

- 📊 Code **complexity**
- 🧩 Code **structure**
- ⚠️ Potential **problem areas**
- 🔍 Nesting depth, branching, function shapes & more

---

## ⭐ Key Features

### 🔍 1. Code Complexity & Hotspot Detection
- Detects long, heavy blocks of code.
- Identifies deep nesting & overly complex sections.
- Helps spot refactoring candidates.

---

### 🧩 2. Structure Analysis
CodeScope evaluates the overall **shape** and **architecture** of your source code.

✔ **Nesting Depth**  
✔ **Branching patterns** (if/else chains, switches)  
✔ **Function / Component size**  
✔ **HTML/JS structure patterns**  
✔ **Inline script detection**  

---

### ⚡ 3. Real-Time Browser Analysis
- Works anywhere — webpages, editors, devtools.
- Zero installation beyond adding the extension.

---

### 🎨 4. Modern UI (React + TypeScript)
- Smooth, clean popup interface.
- Intuitive layout with real-time updates.

---

## 🧰 Architecture Diagram (Mermaid.js)

```mermaid
flowchart TD

A[User Opens Chrome Extension] --> B[Popup React UI]
B --> C[Content Script]
C --> D[Code Analysis Engine - utils/]
D --> E[Nesting Detection]
D --> F[Branch/Structure Analyzer]
D --> G[Function Shape Analyzer]

C --> H[Background Service Worker]

subgraph Frontend (React + TS)
B
end

subgraph Chrome MV3 Scripts
C
H
end

subgraph Analysis Engine
E
F
G
end
```

---

## 📁 Tech Stack

| Layer        | Technology              |
|--------------|-------------------------|
| Frontend     | React, TypeScript       |
| Backend      | Node.js (utility modules) |
| Bundler      | Webpack                 |
| Platform     | Chrome Extension (MV3)  |

---

## 📂 Project Structure

```
CodeScope/
├── Backend/
│   ├── config/
│   ├── controller/
│   ├── routes/
│   ├── schema/
│   ├── utils/
│   ├── Dockerfile
│   ├── docker-compose.yaml
│   ├── app.ts
│   ├── package.json
│   └── tsconfig.json
│
├── src/
│   ├── components/
│   ├── context/
│   ├── utils/
│   ├── App.tsx
│   ├── content.tsx
│   ├── background.ts
│   └── main.tsx
│
├── public/
│   └── index.html
│
├── icons/
│
├── manifest.example.json
├── webpack.config.js
├── package.json
├── pnpm-lock.yaml
├── .gitignore
├── .env.example
└── README.md
```

---

## 🚀 Getting Started

### 1️⃣ Clone
```bash
git clone https://github.com/HariKrishna245/Code-Analyzer-Chrome-Extension.git
cd Code-Analyzer-Chrome-Extension
```

### 2️⃣ Install
```bash
npm install
```

### 3️⃣ Build
```bash
npm run build
```

### 4️⃣ Load Into Chrome
1. Visit `chrome://extensions`
2. Enable **Developer Mode**
3. Click **Load Unpacked**
4. Select the build output folder

---

## 🧭 Roadmap

- 🔘 Improved complexity estimation  
- 🔘 FKGL readability score (planned)  
- 🔘 Interactive charts for complexity  
- 🔘 Inline webpage highlight mode  
- 🔘 Full AST-based analysis  


