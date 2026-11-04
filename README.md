# 🎮 Web & Mobile Community Platform

A feature-rich, interactive web and mobile community platform built with real-time social networking, a virtual economy, embedded HTML5 games, user customization, and push notifications.

> ⚠️ **Disclaimer & Project Status**
>
> This project was created on **November 4, 2026**, and is currently under active development. Some features outlined below may still be in development, incomplete, or pending upcoming updates.

## ✨ Features

### 👤 User Management & Social

* **Authentication**: Secure Login and Sign-Up powered by Firebase Authentication.
* **Avatar Customization**: Personalize user avatars with unlockable cosmetics and limited items.
* **Friend System**: Connect, add friends, and view friend activities.
* **Public Feed & Forums**: Share updates, media, and posts in a Facebook-style social feed alongside structured community discussion forums.

### 💰 Virtual Economy & Gamification

* **Virtual Currency**: Earn currency by playing games and engaging with the platform.
* **Virtual Shop & Marketplace**: Purchase exclusive items, avatar cosmetics, and limited-edition digital collectibles.
* **Loot Boxes**: Open loot boxes to obtain rare and limited items.
* **Item Trading/Reselling**: Users can sell and trade their limited-edition items within the community.

### 🎮 Gaming & Engagement

* **HTML5 Games**: Play built-in browser games directly on the platform.
* **Push Notifications**: Real-time updates and notifications powered by OneSignal.

## 🛠️ Tech Stack & Architecture

* **Frontend & App Wrapping**: HTML, CSS, JavaScript / Frontend Web Framework
* **Database & Backend Services**: [Firebase](https://firebase.google.com/) (Firestore / Realtime Database, Authentication)
* **Deployment & Hosting**: [Vercel](https://vercel.com/)
* **Mobile Application**: Android App built via [FreeWebToAPK](https://www.freewebtoapk.com/)
* **Push Notifications**: [OneSignal](https://onesignal.com/)
* **Version Control**: GitHub

## 🚀 Getting Started

### Prerequisites

Make sure you have the following installed/configured:

* A modern web browser (Chrome, Firefox, Edge, Safari)
* A [Firebase](https://firebase.google.com/) account and project setup

### Local Development Setup

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```

2. **Configure Firebase:**

   * Create a project in the [Firebase Console](https://console.firebase.google.com/).
   * Enable **Authentication** (Email/Password, Google, etc.).
   * Set up **Firestore Database** or **Realtime Database**.
   * Copy your Firebase config object and paste it into your configuration file:

     ```javascript
     const firebaseConfig = {
       apiKey: "YOUR_API_KEY",
       authDomain: "YOUR_AUTH_DOMAIN",
       projectId: "YOUR_PROJECT_ID",
       storageBucket: "YOUR_STORAGE_BUCKET",
       messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
       appId: "YOUR_APP_ID"
     };
     ```

3. **Configure OneSignal Notifications:**

   * Add your OneSignal App ID to the frontend initialization code to enable web push notifications.

4. **Run the Project:**

   * Open `index.html` directly in your browser or serve it using a local server (e.g., Live Server extension in VS Code).

## 🌐 Deployment & Mobile App

### Web Deployment (Vercel)

This repository is configured for automatic deployment with **Vercel**. Any push to the `main` branch will trigger a deployment preview and update the production site.

### Android Application

The Android version of this app is created using **FreeWebToAPK**, wrapping the Vercel-hosted web URL with deep OneSignal push notification integration.

## 🛡️ Security Notes

* Secure all Firebase database read/write rules to prevent unauthorized modification of virtual currency balances or inventory items.
* Run server-side validation (via Firebase Cloud Functions or rule constraints) for transactions involving loot boxes and marketplace sales.

## 🔒 License & Ownership Terms

**Copyright © 2026. All Rights Reserved.**

All code, logic, assets, and design elements within this repository are the sole intellectual property of the author.

By accessing or viewing this repository, you agree to the following terms:

1. **Ownership**: All code in this repository belongs exclusively to the project creator.
2. **No Reuse of Code**: You may **NOT** copy, extract, modify, or reuse any part or snippet of this code in any other project, whether personal, educational, or commercial.
3. **No Public Redistribution**: You may not publicly redistribute, re-license, host, sell, or mirror any portion of this repository.
4. **Permission Required**: If you wish to use or build upon any part of this project, you **must** obtain explicit written permission by reaching out to the author on GitHub.
5.  Permission Required: If you wish to use or build upon any part of this project, you MUST obtain explicit written permission by reaching out to the author via GitHub or directly via email at mcsuwager@gmail.com.
