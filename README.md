# CYPHER - Advanced Safety Monitoring System

An intelligent threat detection and emergency response system built with React that provides real-time voice monitoring, automatic emergency alerts, and location tracking.

video recording - https://drive.google.com/file/d/1Y0beQuXf1OX4ZZbhGZjRpcLmrbJNes72/view?usp=drivesdk
## Features
<img width="1629" height="917" alt="Screenshot 2026-02-22 103312" src="https://github.com/user-attachments/assets/459b7eff-c0fe-4d5b-8413-5c2d9def6738" />
<img width="1464" height="881" alt="Screenshot 2026-02-22 103322" src="https://github.com/user-attachments/assets/71041683-8aa9-4908-aaf3-ccd7b8049e3c" />
<img width="1357" height="927" alt="Screenshot 2026-02-22 103420" src="https://github.com/user-attachments/assets/f1212c59-5e9b-463e-99d9-575cd22d24fa" />

<img width="1880" height="916" alt="Screenshot 2026-02-22 103428" src="https://github.com/user-attachments/assets/9128a2bb-1ebd-4104-9c04-8ef061ead965" />

### 🎯 Real-time Threat Detection
- Voice-activated keyword monitoring using Web Speech API
- Continuous listening mode for instant threat detection
- Customizable trigger keywords

### 🚨 Emergency Response
- Automatic emergency contact alerts via WhatsApp
- Real-time location sharing with Google Maps integration
- Automatic police dispatch notification simulation
- Emergency audio recording with evidence logging

### 📍 Location Tracking
- GPS-based location capture
- Interactive map visualization using Leaflet
- Google Maps integration for emergency sharing
- Real-time coordinate tracking

### 📱 WhatsApp Integration
- Automatic emergency alerts to configured contacts
- Location sharing with map links
- One-click emergency broadcast

### 🎙️ Audio Recording
- Automatic recording when threat is detected
- Evidence storage using IndexedDB
- Playback and management of recorded incidents
- Persistent storage across sessions

## Tech Stack

- **Frontend**: React 18.2.0
- **Speech Recognition**: Web Speech API
- **Maps**: Leaflet.js & Google Maps
- **Storage**: IndexedDB
- **Styling**: Custom CSS with modern UI/UX
- **Build Tool**: React Scripts 5.0.1

## Installation

1. Clone the repository:
```bash
git clone https://github.com/Reyzor255/cypher--TinkHerHack.git
cd cypher--TinkHerHack
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm start
```

The app will open at `http://localhost:3000` (or another port if 3000 is in use).

## Usage

### Setting Up Safety Mode

1. **Configure Trigger Keyword**: Enter a keyword that will activate the emergency response
2. **Add Emergency Contacts**: Input up to 3 emergency contact phone numbers
3. **Enable Safety Mode**: Click "Enable Safety Mode" to start monitoring

### When Threat is Detected

The system automatically:
- Starts recording audio evidence
- Captures your GPS location
- Sends WhatsApp alerts to all emergency contacts
- Displays emergency response confirmation
- Opens the Recording Page with incident details

### Recording Page

- View real-time recording status
- Access location on interactive map
- Share location via WhatsApp
- Review and manage recorded evidence
- Play back or delete recordings

### Map Page

- View incident location on interactive map
- See exact coordinates
- Open location in Google Maps
- Review threat detection details

## Browser Compatibility

- Chrome/Edge (recommended)
- Firefox
- Safari (limited Web Speech API support)

**Requirements**:
- Microphone access permission
- Location services enabled
- Internet connection for maps and WhatsApp

## Privacy & Security

- All recordings stored locally in browser (IndexedDB)
- No data sent to external servers
- Location shared only when threat detected
- User controls all emergency contacts

## Build for Production

```bash
npm run build
```

Creates optimized production build in the `build/` folder.

## Project Structure

```
confirmedcypher/
├── public/
│   └── index.html
├── src/
│   ├── App.js              # Main app component
│   ├── SafetyMonitor.js    # Main monitoring interface
│   ├── RecordingPage.js    # Emergency recording interface
│   ├── MapPage.js          # Location map display
│   └── *.css               # Component styles
├── package.json
└── README.md
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the MIT License.

## Acknowledgments

Built for TinkHerHack - Empowering safety through technology.

---

**⚠️ Important**: This is a safety tool. Always contact local emergency services (911, 112, etc.) in real emergencies.
