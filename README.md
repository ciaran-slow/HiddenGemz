<p align="center">
  <img src="https://res.cloudinary.com/dnl6b6gaq/image/upload/v1776291443/ReadmeImage_mibsap.png" width="100%">
</p>

# HiddenGemz 💎

HiddenGemz is a full-stack community-driven platform designed to help you discover, share, and save the best local spots. Whether it's a quiet cafe, a bustling bar, or a hidden restaurant, HiddenGemz connects you with authentic local experiences.

**Live demo:** https://hidden-gemz-nz.onrender.com/ *(hosted on a free tier, so the first load can take about 20 seconds)*

> A team project built by five developers during the Dev Academy Aotearoa full-stack programme. This repository is a copy of the team's original repo, which lives in the course organisation's private account, so its commit history is flattened here.

## 🚀 Features

-   **Discover:** Browse a curated list of local "gemz" with detailed reviews and interactive maps.
-   **Search & Filter:** Find exactly what you're looking for by suburb, venue type, or specific amenities (Pet Friendly, Vegan, Outdoor seating, etc.).
-   **Community Contributions:** Share your own favourite spots by adding new posts with photos, reviews, and tags.
-   **Personalized Profiles:** Track your own contributions and manage the spots you've shared.
-   **Favourites:** Save your must-visit spots to your personal favourites list.
-   **Follow System:** Follow other "Gem Hunters" to keep up with their latest discoveries.
-   **Authentication:** Secure login and profile management powered by Auth0.
-   **Interactive Maps:** View exact locations using integrated Google Maps.

## 🛠️ Tech Stack

### Frontend
-   **React** (v18) with **TypeScript**
-   **Vite** for fast development and bundling
-   **Tailwind CSS** for modern, responsive styling
-   **TanStack Query** (React Query) for efficient data fetching and caching
-   **React Router** (v7) for seamless navigation
-   **React Hot Toast** for beautiful notifications

### Backend
-   **Node.js** & **Express.js**
-   **Knex.js** (Query Builder)
-   **SQLite3** (Development) & **PostgreSQL** (Production)
-   **Auth0** for secure JWT-based authentication

---

## 🙋 My contributions (Ciaran)

I was one of five contributors, with 53 commits and 34 merged pull requests in the team repo. My work covered:

- **Project start:** the routing skeleton, and the first post cards and detail modal.
- **Authentication in the UI:** Auth0 login on the front end, the profile pages and a "my profile" view.
- **Posts:** image upload with Cloudinary, edit and delete flows, and form and filter styling and fixes.
- **Community features:** comments (with optimistic updates), favourites and favourite counts, and a follow/friend system.
- **Maps:** an embedded map in the post modal.
- **Polish:** loading, empty-result and back-button states, search and sort fixes, and mobile fixes.
- **Deployment:** the Render setup and the database fixes needed to get it live.
- **Docs:** the README and its hero image.

---

## ⚙️ Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/ciaran-slow/HiddenGemz.git
cd HiddenGemz
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Database Setup
HiddenGemz uses Knex for migrations and seeds. 

**Run Migrations:**
```bash
npm run knex migrate:latest
```

**Run Seeds:**
```bash
npm run knex seed:run
```

### 4. Environment Variables
Create a `.env` file in the root directory and add your Auth0 and Cloudinary credentials:
```env
VITE_AUTH0_DOMAIN=your_auth0_domain
VITE_AUTH0_CLIENT_ID=your_auth0_client_id
VITE_AUTH0_AUDIENCE=your_auth0_audience
VITE_CLOUDINARY_CLOUD_NAME=your_cloudinary_name
VITE_CLOUDINARY_UPLOAD_PRESET=your_upload_preset
```

### 5. Run the Application
Start both the client and server in development mode:
```bash
npm run dev
```
-   **Frontend:** `http://localhost:5173`
-   **Backend:** `http://localhost:3000`

---

## 👥 Contributors

Meet the team behind HiddenGemz:

-   **Ciaran S** - [GitHub Profile](https://github.com/ciaran-slow)
-   **Johnny C** - [GitHub Profile](https://github.com/johnny-cassin)
-   **Jay H** - [GitHub Profile](https://github.com/JayHuston-Dev)
-   **Phoebe H** - [GitHub Profile](https://github.com/PhoebeHuPing)
-   **Melia G** - [GitHub Profile](https://github.com/melia-gratsounas)

---

## 📄 License
This project is licensed under the MIT License - see the [package.json](package.json) file for details.
