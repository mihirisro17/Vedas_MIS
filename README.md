<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=200&section=header&text=VEDAS%20MIS&fontSize=80&fontColor=fff&animation=twinkling&fontAlignY=35&desc=Management%20Information%20System&descAlignY=55&descSize=24" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=6366F1&center=true&vCenter=true&multiline=true&width=800&height=120&lines=🛰️+Comprehensive+Monitoring+%26+Analytics+Dashboard;🌍+Servers+%7C+Services+%7C+Alerts+%7C+Satellite+Data;⚡+Real-Time+Socket.IO+%7C+Vue.js+3" alt="Typing SVG" />

<br/>

![Vue.js](https://img.shields.io/badge/Vue.js-3-42b883?style=for-the-badge&logo=vue.js&logoColor=white)
![Socket.IO](https://img.shields.io/badge/Socket.IO-4.8.1-010101?style=for-the-badge&logo=socket.io&logoColor=white)
![ISRO](https://img.shields.io/badge/SAC%2FISRO-Government%20of%20India-FF9933?style=for-the-badge&logo=nasa&logoColor=white)
![Status](https://img.shields.io/badge/Status-Live-10b981?style=for-the-badge&logo=statuspage&logoColor=white)
![Real-Time](https://img.shields.io/badge/Real--Time-Monitoring-6366f1?style=for-the-badge&logo=grafana&logoColor=white)

</div>

---

## 🌌 Overview

**VEDAS MIS** is a real-time **Management Information System** dashboard built for **VEDAS (Visualisation of Earth observation Data and Archival System)** at **Space Applications Centre (SAC), ISRO**. It provides a unified command center for monitoring satellite data pipelines, server infrastructure, services, and processing workflows — all from a single animated interface.

---

## ✨ Features

<table>
<tr>
<td width="50%">

### 🖥️ Infrastructure Monitoring
- **Server Monitor** — Track server health & uptime
- **Service Monitor** — Data pipeline status
- **Service Monitor New** — Plugin-based monitoring framework
- **Processing Script Monitor** — Script health checks
- **Data Chain Monitoring** — Satellite tracking
- **Pool Group Health** — Storage pool analytics
- **Raster Error Logs** — Publish error detection

</td>
<td width="50%">

### 📊 Analytics & Tools
- **Team Analytics** — Performance metrics
- **Ridam Pool Analytics** — Pool storage analytics
- **Publish Monitoring** — Dataset publisher status
- **Geoentity Monitoring** — Geo data tracking
- **Ridam Registration** — Tool management

</td>
</tr>
</table>

---

## 🚨 Real-Time Alert System

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=15&pause=800&color=EF4444&center=true&vCenter=true&width=700&lines=🔴+OFFLINE+—+Server+Down+Alert;🔴+MEMORY+100%25+—+RAM+Critical;🔴+CPU+—+Critical+Load;🟠+STORAGE+100%25+—+Disk+Full+Warning;🔵+INFO+—+System+Notification;🟣+API+ERROR+—+Endpoint+Failure" alt="Alert Types" />

</div>

| Alert Type | Severity | Color | Audio |
|---|---|---|---|
| `OFFLINE` | 🔴 Critical | Red Pulse | 3× Sawtooth Buzz |
| `MEMORY 100%` | 🔴 Critical | Red Pulse | 3× Sawtooth Buzz |
| `CPU` | 🔴 Critical | Red Pulse | 3× Sawtooth Buzz |
| `STORAGE 100%` | 🟠 Warning | Orange Pulse | 2× Triangle Tone |
| `DISK` | 🟠 Warning | Orange Pulse | 2× Triangle Tone |
| `INFO` | 🔵 Info | Blue Pulse | Soft Sine Ping |
| `API ERROR` | 🟣 Error | Purple Pulse | 3× Sawtooth Buzz |

> 🚨 **Server Critical Alarm** — Full-screen red banner with a siren animation, countdown timer (10s), and an Acknowledge button.

---

## 🎨 Themes

| Theme | Preview | Description |
|---|---|---|
| 🇮🇳 **VEDAS** | Saffron · White · Green | Indian tricolor — default theme |
| 🌑 **Dark** | Deep navy & indigo | Sleek dark mode |
| 🌊 **Ocean** | Cyan & sky blue | Refreshing ocean palette |
| 🌿 **Forest** | Emerald & teal | Nature-inspired greens |
| 🌅 **Sunset** | Amber, orange & red | Warm evening tones |
| 🤖 **Auto** | Time-adaptive | Morning ☀️ / Afternoon 🌤️ / Evening 🌆 / Night 🌙 |

---

## 🌞 Solar System Home Screen

The home page features a **fully animated interactive solar system**:

- ☀️ Rotating & pulsing **Sun** with radial glow
- 🪐 All 8 planets (**Mercury → Neptune**) orbiting in real-time
- 🌙 **Moon** orbiting Earth on its own orbit
- ☄️ **Asteroid belt** rotating around the Mars orbit
- 🚀 Two animated **rockets** crossing the screen
- 🛰️ Floating **satellite** & **comet** decorations
- ⭐ Floating **stars** with opacity animations

---

## ⏰ Smart Break Notifications

| Time | Icon | Title | Message |
|---|---|---|---|
| **10:30 AM** | ☕ | Tea Break! | Time for a refreshing cup of tea! |
| **12:30 PM** | 🍽️ | Lunch Time! | Enjoy your meal and recharge! |
| **3:00 PM** | 🍪 | Evening Snacks! | Take a break and have some snacks! |
| **5:30 PM** | 🏠 | Office Time is Over! | Great work today! Time to head home! |

> Auto-closes after **150 seconds** with a visible countdown. Resets daily at midnight.

---

## 🏗️ Architecture
```/text
VEDAS MIS
├── 🖥️ Frontend → Vue.js 3 (CDN), Inter Font, CSS Animations
├── ⚡ Real-Time → Socket.IO 4.8.1 (WebSocket + Polling fallback)
├── 📡 Backend → http://192.168.2.137:8080 (SAC Internal Network)
├── 🔔 Alert Engine → Web Audio API (Sawtooth / Triangle / Sine waves)
├── 🎨 Themes → CSS Custom Properties (8 themes + auto time-based)
└── 📊 Dashboards → Embedded iframes per monitoring app
```

---

## 📡 Socket.IO Events

| Event | Direction | Description |
|---|---|---|
| `new_alert` | Server → Client | Generic new alert |
| `server_alert` | Server → Client | Server category alert |
| `dataset_alert` | Server → Client | Dataset pipeline alert |
| `process_alert` | Server → Client | Processing script alert |
| `storage_alert` | Server → Client | Storage/disk alert |
| `alert_cleared` | Server → Client | Remove a specific alert |
| `clear_alerts` | Server → Client | Clear all or by category |
| `update_stats` | Server → Client | Update server/service counts |
| `initial_alerts` | Server → Client | Bootstrap alerts on connect |

---

## 🚀 Getting Started

```bash
# 1. Clone or place index.html in your project directory

# 2. Serve the file locally
python -m http.server 8000
# OR
npx serve .

# 3. Open in browser
open http://localhost:8000/index.html
```

> 💡 The dashboard runs in **demo mode** without a Socket.IO backend. For live alerts, connect to the SAC internal server at `http://192.168.2.137:8080`.

---

## 📁 Monitored Applications

<details>
<summary>📋 Click to expand full application list</summary>

| Icon | Name | Category | Description | Endpoint |
|---|---|---|---|---|
| 🖥️ | Server Monitor | Monitoring | Infrastructure Status | `/monitoring/server/home` |
| ⚙️ | Service Monitor | Monitoring | Data Pipeline Status | `/monitoring/datasets` |
| 🔌 | Service Monitor New | Monitoring | Plugin-based framework | `/vedas/servicemonitoring` |
| 📜 | Processing Script Monitor | Monitoring | Script Health Check | `/processmonitoring` |
| 🛰️ | Data Chain Monitoring | Monitoring | Satellite Tracking | `/monitoring/sentinel` |
| 📤 | Publish Monitoring | Monitoring | Dataset Publisher | `/ridam/datasetpublisher` |
| 📊 | Ridam Pool Analytics | Monitoring | Pool Storage Analytics | `/poolstoragemonitoring` |
| 🏥 | Pool Group Health | Monitoring | Group Health Status | `/monitoring/health` |
| 🗺️ | Geoentity Monitoring | Monitoring | Geo Data Tracking | `/geoentitymonitoring` |
| 🔍 | Raster Error Logs | Monitoring | Publish Error Detection | `/ridam/errorlogs` |
| 📈 | Team Analytics | Analytics | Performance Metrics | `/taskboard/dashboard` |
| 🔧 | Ridam Registration | Tools | Tool Management | `/ridam/registration` |

</details>

---

## 🛠️ Tech Stack

<div align="center">

![Vue.js](https://img.shields.io/badge/Vue.js-42b883?style=flat-square&logo=vue.js&logoColor=white)
![Socket.IO](https://img.shields.io/badge/Socket.IO-010101?style=flat-square&logo=socket.io&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS_Animations-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Web Audio API](https://img.shields.io/badge/Web_Audio_API-FF6B35?style=flat-square&logo=googlechrome&logoColor=white)
![Google Fonts](https://img.shields.io/badge/Inter_Font-4285F4?style=flat-square&logo=google-fonts&logoColor=white)

</div>

---

<div align="center">

**Developed & Maintained at**

**Space Applications Centre (SAC) · ISRO · Government of India**

© 2025 VEDAS · All Rights Reserved

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=100&section=footer&text=VEDAS+%7C+SAC+%7C+ISRO&fontSize=20&fontColor=fff&animation=twinkling&fontAlignY=65" width="100%"/>

</div>
