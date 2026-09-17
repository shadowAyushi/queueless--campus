# 🎓 QueueLess Campus

> **Smart Campus Virtual Queue Management System**  
> *Stop Waiting. Start Living.*

QueueLess Campus eliminates physical lines at busy college service counters (Canteen, Photocopy/Xerox, Central Library, Administration Office, Fees & Accounts, and Transport/Bus Pass). Students can check live counter traffic, claim a virtual token from anywhere on campus, track their position in real time, and receive smart proximity audio/visual alerts when their turn is approaching.

---

## 🌟 Key Features

### 1. Student Dashboard & Directory
- Real-time queue volume, dynamic wait times, and current token being served.
- Traffic badges: **Low**, **Moderate**, and **Busy**.
- 6 Campus Services:
  - 🍔 **Campus Canteen & Cafe** (Counter A)
  - 🖨️ **Photocopy & Xerox Center** (Counter X)
  - 📚 **Central Library Circulation** (Counter L)
  - 🏢 **Administration Office** (Counter D)
  - 💳 **Fees & Accounts Counter** (Counter F)
  - 🚌 **Transport & Bus Pass Desk** (Counter T)
- Live search and category filters.

### 2. Virtual Token Pass System
- Authentic digital boarding pass with simulated QR code, token numbers (e.g. `A118`, `X052`), timestamp, and counter name.
- Live countdown: **"11 people ahead"**, **"~18 min wait"**, **"Now serving: A106"**.
- Real-time progress bar showing queue drain rate.
- Safe cancellation ("Leave Queue") flow with confirmation.

### 3. Proactive In-App Notifications & Sound Chimes
- Turn approaching alert when 3 students remain ahead.
- Native airport counter two-tone chime synthesized via the browser's **Web Audio API** (zero external MP3 dependencies).
- Confetti celebration upon reaching the counter.
- Non-intrusive, stackable toast notifications.

### 4. Admin & Counter Staff Console
- Counter switcher to manage any campus counter.
- Hero **Now Serving** display with active student pulse.
- Controls: **[CALL NEXT]**, **[COMPLETE]**, **[SKIP TOKEN]**, and **[PAUSE / RESUME QUEUE]**.
- Dynamic service pacing slider (0.5 – 8.0 min/student) which dynamically recalculates wait times across all student passes.
- Walk-in token generator for students without smartphones.

### 5. Campus Analytics & Smart Queue Prediction
- Aggregate metrics: Average campus wait time, total served today, peak rush hours.
- Recharts visualizations: Queue volume over time and tokens served by counter.
- **Smart Queue Prediction**: Machine-simulated congestion forecasts for every hour of the day, optimal visiting windows, and peak rush warnings.

### 6. Hackathon Judge Demo Toolkit (`DemoBar`)
- **Auto Sim**: Automatically calls tokens every 6 seconds so judges can watch queues advance and notifications fire in real-time.
- **Call Next**: Advance single token.
- **Test Alert**: Fires turn approaching proximity ping with chime.
- **Sim Rush**: Floods queues with 15 students to demonstrate high-traffic handling.
- **Reset**: 1-click restoration to default seed data.

---

## 🛠️ Tech Stack

- **Framework**: React 19 + TypeScript
- **Build Tool**: Vite
- **Styling**: Tailwind CSS
- **Icons**: Lucide React
- **Charts**: Recharts
- **Celebration Effects**: Canvas Confetti
- **Audio Synthesis**: Native Web Audio API (Sine wave oscillator chime)
- **Persistence**: `localStorage` with reactive multi-tab synchronization

---

## 🚀 Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) (v18 or higher recommended)
- Git

### Installation & Local Run
```bash
# 1. Clone repository
git clone https://github.com/YOUR_USERNAME/queueless-campus.git
cd queueless-campus

# 2. Install dependencies
npm install

# 3. Start development server
npm run dev
```

Open your browser and visit:
`http://localhost:5173/`

### Build for Production
```bash
npm run build
```
Production assets will be built to the `dist/` directory.

---

## 📄 License
MIT License. Built for University Hackathon 2026.
