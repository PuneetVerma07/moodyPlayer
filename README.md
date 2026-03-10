# 🎵 moodyPlayer - AI-Powered Mood-Based Music Recommendation

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![MERN Stack](https://img.shields.io/badge/Stack-MERN-blue.svg)](https://www.mongodb.com/mern-stack)
[![AI-Powered](https://img.shields.io/badge/AI-Face%20API-red.svg)](https://justadudewhohacks.github.io/face-api.js/docs/index.html)

**moodyPlayer** is an innovative web application that detects a user's current mood via real-time facial recognition and serves a curated playlist of songs that match their emotional state. Stop scrolling through playlists—let your face do the talking!

---

## 🚀 Key Features

- **Real-time Emotion Detection:** Uses `face-api.js` to capture and analyze facial expressions through the webcam.
- **Dynamic Playlists:** Intelligent backend logic that maps detected moods (Happy, Sad, Angry, Neutral, etc.) to specific music categories.
- **MERN Architecture:** Robust full-stack implementation with a scalable Node/Express backend and a responsive React frontend.
- **Seamless API Integration:** Custom-built APIs to fetch and display song data based on the identified mood.

---

## 🛠️ Tech Stack

**Frontend:**
- **React.js:** Component-based UI architecture.
- **Face-api.js:** Browser-based AI for facial landmark and emotion detection.
- **CSS3/Tailwind:** (Add if applicable) For a sleek, modern user interface.

**Backend:**
- **Node.js & Express.js:** Scalable server-side logic and RESTful API development.
- **MongoDB:** Database for storing song metadata and user preferences.

**Tools & Others:**
- **Axios:** For handling asynchronous API requests.
- **Git/GitHub:** Version control.

---

## 📸 How it Works

1. **Capture:** The app requests camera access to detect facial features.
2. **Analyze:** The AI model processes the image to determine the dominant emotion.
3. **Fetch:** The frontend sends the mood data to the `/api/songs` endpoint.
4. **Play:** A filtered list of songs is returned and displayed for the user to enjoy.

---

## 🛣️ API Endpoints (Development)

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `POST` | `/api/mood/detect` | Sends facial data/mood to the server. |
| `GET` | `/api/songs/:mood` | Returns a list of songs filtered by the mood parameter. |

---

## 🛠️ Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/PuneetVerma07/moodyPlayer.git](https://github.com/PuneetVerma07/moodyPlayer.git)

2. **Install Dependencies (Backend):**
    ```bash
    cd backend
    npm install

3. **Install Dependencies (Frontend):**
   ```bash
   cd ../frontend
   npm install

4. **Environment Variables:** Create a .env file in the backend folder and add your MONGODB_URI.

5. **Run the app:**
   ```bash
   # In backend folder
    npm start
    # In frontend folder
    npm start
