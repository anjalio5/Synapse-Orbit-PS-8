Orbit is a polished, student-focused wellness application designed to support mental health and community engagement through AI-driven companionship, daily missions, and anonymous social interactions.

## 🌟 Key Features

- **Nova AI Companion**: A personal AI guide powered by Google's Gemini, providing empathetic support and wellness tracking.
- **Mood Hub**: Track your emotional well-being over time with intuitive check-ins.
- **Daily Missions**: Engaging, actionable tasks designed to build healthy habits and boost student morale.
- **Support Hub**: An anonymous space for students to share experiences, seek advice, and support one another.
- **Avatar Personalization**: Create and customize a digital representative for your wellness journey.
- **Orb Island**: A gamified visual representation of your progress and mental state.
- **Profile & Progress**: Comprehensive tracking of your missions, submissions, and wellness stats.

## 🛠️ Tech Stack

- **Frontend**: React 19 (Vite)
- **Styling**: Tailwind CSS (v4)
- **Animations**: Motion (formerly Framer Motion)
- **AI Engine**: Google Gemini API (`@google/genai`)
- **Backend/Auth**: Firebase (Authentication & Firestore)
- **Real-time/Database**: Supabase
- **Icons**: Lucide React
- **Routing**: React Router 7

## 📁 Project Structure

- `src/screens/`: Individual page components (Onboarding, Hub, Chat, Missions, etc.)
- `src/components/`: Reusable UI components like `BottomNav`.
- `src/lib/`: Unified service initializations for Firebase and Supabase.
- `src/data/`: Static assets and configuration data.
- `public/`: Avatars and other static image assets.

## 🚀 Getting Started

### 1. Prerequisites
- Node.js (Latest LTS recommended)
- Firebase Project (with Anonymous and Google Auth enabled)
- Supabase Project
- Gemini API Key

### 2. Installation
```bash
npm install
```

### 3. Environment Configuration
Create a `.env` file based on `.env.example`:
```env
GEMINI_API_KEY="your_gemini_api_key"
APP_URL="http://localhost:3000"
VITE_SUPABASE_URL="your_supabase_url"
VITE_SUPABASE_ANON_KEY="your_supabase_anon_key"
```

### 4. Firebase Setup
Ensure `firebase-applet-config.json` is updated with your real project credentials.

### 5. Running the App
```bash
npm run dev
```
The app will be available at `http://localhost:3000`.

## 📜 Development Notes

- **Design System**: The app follows a "Swiss/Modern" aesthetic with a warm, approachable color palette (`#fdfaf8` background).
- **Mobile First**: Optimized for a 400px width "App" container, providing a native-like experience even in the browser.
- **AI Integration**: Chat history and mood analysis are processed client-side via the Gemini API for privacy and responsiveness.

## 🛡️ Privacy & Security
- **Anonymous Entry**: Users can start their journey anonymously via Firebase Anonymous Auth.
- **Data Isolation**: Support Hub interactions are designed to be community-driven while maintaining student anonymity.
