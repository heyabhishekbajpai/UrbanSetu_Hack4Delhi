# UrbanSetu - External Integrations & Dependencies

This document lists all external APIs, services, libraries, and assets used in the UrbanSetu application.

## 1. External APIs & Services

| Service | Purpose | URL / Endpoint |
| :--- | :--- | :--- |
| **Supabase** | Backend (Auth, DB, Storage) | `https://<your-project-ref>.supabase.co` |
| **OpenStreetMap Nominatim** | Reverse Geocoding (Lat/Long to Address) | `https://nominatim.openstreetmap.org/reverse` |
| **BigDataCloud** | Reverse Geocoding (Backup) | `https://api.bigdatacloud.net/data/reverse-geocode-client` |
| **OpenStreetMap Tiles** | Map Visualizations | `https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png` |
| **Teachable Machine** | AI Model Hosting (Fallback) | `https://teachablemachine.withgoogle.com/models/FzFLbZLp9f/` |
| **Via Placeholder** | Placeholder Images | `https://via.placeholder.com` |

## 2. Key Libraries & Packages

| Package | Version | Purpose |
| :--- | :--- | :--- |
| `@supabase/supabase-js` | `^2.89.0` | Client library for Supabase interaction. |
| `@teachablemachine/image` | `^0.8.5` | Client-side image classification using Teachable Machine models. |
| `@tensorflow/tfjs` | `1.3.1` | Required peer dependency for Teachable Machine. |
| `leaflet` & `react-leaflet` | `^1.9.3` / `^4.2.1` | Interactive maps for dashboard and reporting. |
| `react-hook-form` | `^7.43.0` | Efficient form validation and handling. |
| `framer-motion` | `^10.0.0` | Animation library for smooth UI transitions. |
| `lucide-react` | `^0.263.1` | Icon set used throughout the application. |
| `react-hot-toast` | `^2.4.0` | Toast notifications for user feedback. |
| `date-fns` | `^2.29.3` | Date manipulation and formatting. |

## 3. External Assets

The application loads some static assets directly from the GitHub repository:

*   **Logos**:
    *   `https://raw.githubusercontent.com/heyabhishekbajpai/UrbanSetu/main/public/logo.png`
    *   `https://raw.githubusercontent.com/heyabhishekbajpai/UrbanSetu/main/public/logodark.png`
*   **Mock Images**:
    *   `https://raw.githubusercontent.com/heyabhishekbajpai/UrbanSetu/main/public/garbage.png`
    *   `https://raw.githubusercontent.com/heyabhishekbajpai/UrbanSetu/main/public/pothole.jpg`

## 4. Browser APIs Used

*   **Geolocation API**: (`navigator.geolocation`) Used to get the user's current coordinates for reporting.
*   **MediaDevices API**: (`navigator.mediaDevices.getUserMedia`) Used to access the camera for capturing complaint photos.
*   **SpeechRecognition API**: (`window.SpeechRecognition` / `window.webkitSpeechRecognition`) Used for voice-to-text description input.
