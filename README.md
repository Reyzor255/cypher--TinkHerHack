<p align="center">
  <img src="./img.png" alt="CYPHER Banner" width="100%">
</p>

# CYPHER - Advanced Safety Monitoring System 🎯

## Basic Details

### Team Name: [Your Team Name]

### Team Members
- Member 1: [Name] - [College]
- Member 2: [Name] - [College]

### Hosted Project Link
[Your hosted link here]

### Project Description
CYPHER is an intelligent threat detection and emergency response system that provides real-time voice monitoring, automatic emergency alerts via WhatsApp, and GPS location tracking to ensure personal safety in critical situations.

### The Problem Statement
In emergency situations, victims often cannot make phone calls or send messages for help. Traditional safety apps require manual activation, which may not be possible when under threat. There's a critical need for an automated system that can detect danger and alert emergency contacts without user intervention.

### The Solution
CYPHER uses continuous voice monitoring with Web Speech API to detect customizable trigger keywords. When a threat is detected, it automatically records audio evidence, captures GPS location, and sends WhatsApp alerts with location links to pre-configured emergency contacts - all without requiring any manual action from the user.

---

## Technical Details

### Technologies/Components Used

**For Software:**
- Languages used: JavaScript (ES6+), HTML5, CSS3
- Frameworks used: React 18.2.0
- Libraries used: Leaflet.js (Maps), Web Speech API, IndexedDB
- Tools used: React Scripts 5.0.1, npm, Git

---

video recording - https://drive.google.com/file/d/1Y0beQuXf1OX4ZZbhGZjRpcLmrbJNes72/view?usp=drivesdk
## Features
<img width="1629" height="917" alt="Screenshot 2026-02-22 103312" src="https://github.com/user-attachments/assets/459b7eff-c0fe-4d5b-8413-5c2d9def6738" />
<img width="1464" height="881" alt="Screenshot 2026-02-22 103322" src="https://github.com/user-attachments/assets/71041683-8aa9-4908-aaf3-ccd7b8049e3c" />
<img width="1357" height="927" alt="Screenshot 2026-02-22 103420" src="https://github.com/user-attachments/assets/f1212c59-5e9b-463e-99d9-575cd22d24fa" />

<img width="1880" height="916" alt="Screenshot 2026-02-22 103428" src="https://github.com/user-attachments/assets/9128a2bb-1ebd-4104-9c04-8ef061ead965" />

- **Real-time Voice Monitoring**: Continuous listening mode using Web Speech API for instant threat detection
- **Automatic Emergency Response**: Sends WhatsApp alerts to multiple contacts with location when threat detected
- **GPS Location Tracking**: Real-time location capture with interactive Leaflet maps and Google Maps integration
- **Audio Evidence Recording**: Automatic recording with IndexedDB storage for incident documentation
- **Multi-Contact Alert System**: Configure up to 3 emergency contacts for simultaneous alerts
- **Interactive Map Visualization**: View incident locations with coordinates and map links

---

## Implementation

### For Software:

#### Installation
```bash
git clone https://github.com/Reyzor255/cypher--TinkHerHack.git
cd cypher--TinkHerHack
npm install
```

#### Run
```bash
npm start
```

The app will open at `http://localhost:3000`

---

## Project Documentation

### For Software:

#### Screenshots

![Main Dashboard](screenshots/dashboard.png)
*CYPHER main monitoring interface with safety mode controls and emergency contact configuration*

![Recording Page](screenshots/recording.png)
*Emergency recording interface showing active recording, location sharing, and evidence log*

![Map View](screenshots/map.png)
*Interactive map displaying incident location with coordinates and Google Maps integration*

#### Diagrams

**System Architecture:**

```
┌─────────────────────────────────────────────────────────┐
│                    CYPHER System                         │
├─────────────────────────────────────────────────────────┤
│                                                          │
│  ┌──────────────┐      ┌──────────────┐                │
│  │ Web Speech   │─────▶│   Keyword    │                │
│  │     API      │      │   Detection  │                │
│  └──────────────┘      └──────┬───────┘                │
│                               │                          │
│                               ▼                          │
│                    ┌──────────────────┐                 │
│                    │  Threat Detected │                 │
│                    └────────┬─────────┘                 │
│                             │                            │
│          ┌──────────────────┼──────────────────┐        │
│          ▼                  ▼                  ▼         │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐ │
│  │   Audio      │  │  GPS/Maps    │  │  WhatsApp    │ │
│  │  Recording   │  │   Location   │  │   Alerts     │ │
│  │  (IndexedDB) │  │  (Leaflet)   │  │  (wa.me)     │ │
│  └──────────────┘  └──────────────┘  └──────────────┘ │
│                                                          │
└─────────────────────────────────────────────────────────┘
```

**Application Workflow:**

```
User Opens App
      │
      ▼
Configure Keyword & Contacts
      │
      ▼
Enable Safety Mode
      │
      ▼
Continuous Voice Monitoring ◄─────┐
      │                            │
      ▼                            │
Keyword Detected? ─── NO ─────────┘
      │
     YES
      │
      ├─────▶ Start Audio Recording
      │
      ├─────▶ Capture GPS Location
      │
      ├─────▶ Send WhatsApp Alerts
      │
      ▼
Open Recording Page
      │
      ├─────▶ View/Manage Recordings
      │
      ├─────▶ View Location on Map
      │
      └─────▶ Share Location
```

---

## Project Demo

### Video
[Add your demo video link here]

*Demo showcases: Voice detection triggering emergency response, automatic WhatsApp alerts with location, audio recording, and interactive map visualization*

### Additional Demos
- Live Demo: [Your hosted link]
- APK Download: [If applicable]

---

## Browser Compatibility & Requirements

**Supported Browsers:**
- Chrome/Edge (Recommended)
- Firefox
- Safari (Limited Web Speech API support)

**Required Permissions:**
- Microphone access
- Location services
- Internet connection (for maps and WhatsApp)

---

## Privacy & Security

- All recordings stored locally in browser (IndexedDB)
- No data sent to external servers
- Location shared only when threat detected
- User controls all emergency contacts
- No backend server or database required

---

## Team Contributions

- [Name 1]: Frontend development, Speech recognition integration, UI/UX design
- [Name 2]: Location tracking, Map integration, WhatsApp alert system, IndexedDB implementation

---

## AI Tools Used (Optional - For Transparency Bonus)

**Tool Used:** [If applicable - e.g., GitHub Copilot, ChatGPT]

**Purpose:**
- Code optimization and debugging assistance
- Component structure suggestions
- CSS styling improvements

**Percentage of AI-generated code:** Approximately 15%

**Human Contributions:**
- Complete architecture design and planning
- Core business logic (speech recognition, location tracking, alert system)
- Integration of all components
- UI/UX design and implementation
- Testing and debugging

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

Built for TinkHerHack - Empowering safety through technology.

**⚠️ Important Disclaimer:** This is a safety tool designed to assist in emergencies. Always contact local emergency services (911, 112, etc.) in real emergencies. This app should be used as a supplementary safety measure, not a replacement for professional emergency services.

---

Made with ❤️ at TinkerHub
