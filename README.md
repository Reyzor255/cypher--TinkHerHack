

# CYPHER - Advanced Safety Monitoring System 🎯
<img width="1280" height="640" alt="img" src="https://github.com/user-attachments/assets/51755682-17a7-4611-851b-619c27b8de26" />


## Basic Details

### Team Name:Athena

### Team Members
- Member 1: Reyhan Hazeem - Toc H institute of Techonolgy 
- Member 2: Santra Alexander - Toc H institute of Technology

### Hosted Project Link
https://cypher-eight-nu.vercel.app/

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


## Features


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
<img width="1629" height="917" alt="Screenshot 2026-02-22 103312" src="https://github.com/user-attachments/assets/b70e0bdc-51f4-414e-a886-14385682ae3c" />

<img width="1464" height="881" alt="Screenshot 2026-02-22 103322" src="https://github.com/user-attachments/assets/109d7045-9d70-4394-8785-ac2b457dd7ed" />

<img width="1357" height="927" alt="Screenshot 2026-02-22 103420" src="https://github.com/user-attachments/assets/8ad704a2-f9b8-4b94-a47f-a79d1794651a" />
<img width="1880" height="916" alt="Screenshot 2026-02-22 103428" src="https://github.com/user-attachments/assets/b20701f5-83bb-4412-b7c2-1fd702a23d0e" />

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
video recording - https://drive.google.com/file/d/1Y0beQuXf1OX4ZZbhGZjRpcLmrbJNes72/view?usp=drivesdk

*Demo showcases: Voice detection triggering emergency response, automatic WhatsApp alerts with location, audio recording, and interactive map visualization*




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

- Santra Alexander: Frontend development, Speech recognition integration, UI/UX design
- Reyhan Hazeem: Location tracking, Map integration, WhatsApp alert system, IndexedDB implementation

---

## AI Tools Used (Optional - For Transparency Bonus)

**Tool Used:** chatgpt, gemini, amazon q

**Purpose:**
- Code optimization and debugging assistance
- Component structure suggestions
- CSS styling improvements



**Human Contributions:**
- Complete architecture design and planning
- Core business logic (speech recognition, location tracking, alert system)
- Integration of all components

- Testing and debugging

---

## License

This project is licensed under the MIT License - 

---

## Acknowledgments

Built for TinkHerHack - Empowering safety through technology.

**⚠️ Important Disclaimer:** This is a safety tool designed to assist in emergencies. Always contact local emergency services (911, 112, etc.) in real emergencies. This app should be used as a supplementary safety measure, not a replacement for professional emergency services.

---

Made with ❤️ at TinkerHub
