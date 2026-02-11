# SOSMate – Personal Safety Android Application

SOSMate is an Android-based personal safety application developed to provide rapid emergency assistance and real-time protection. The system is designed to enhance personal security, particularly for women and vulnerable individuals, by enabling instant distress alerts, live location tracking, and discreet emergency features.

The application combines user-triggered emergency tools with continuous background monitoring to ensure help can be reached quickly during critical situations.

---

## Project Objective

The goal of SOSMate is to create a dependable mobile safety companion that:

- Reduces emergency response time  
- Shares accurate real-time location during distress  
- Provides discreet escape options in unsafe environments  
- Operates reliably even when the app is not actively open  

---

## Key Features

### One-Touch SOS Activation
A dedicated SOS button on the main dashboard allows users to instantly trigger emergency alerts.

### Power Button Emergency Trigger
Users can discreetly activate the SOS alert by pressing the device power button three consecutive times, even when the device is locked.

### Automatic Emergency SMS
When SOS is activated, the app automatically sends an SMS to all registered emergency contacts containing:
- A distress alert message  
- A Google Maps link showing the user’s live location  

### Real-Time Location Tracking
Uses Google Play Services Location API to continuously monitor and update GPS location during emergency mode.

### Fake Call Simulation
Allows users to simulate an incoming phone call, helping them safely exit uncomfortable or potentially threatening situations.

### Background Safety Services
Persistent background services ensure uninterrupted protection:
- Auto-start on device reboot  
- Continuous tracking during SOS mode  
- Monitoring for hardware-triggered alerts  

### Location History
Maintains a timestamped record of previously captured locations, allowing users to review movement history if required.

### Emergency Contact Management
Users can add, edit, and remove emergency contacts. At least one contact must be registered to enable SOS functionality.

---

## Technical Stack

| Component | Technology |
|----------|------------|
| Operating System | Android 8.0 (Oreo) and above |
| Programming Language | Java |
| UI Design | XML Layouts |
| IDE | Android Studio |
| Build System | Gradle |
| Database | SQLite |
| APIs | Google Play Services Location API, Google Maps API |
| Libraries | AndroidX, Material Design Components |

---

## System Architecture

SOSMate follows a modular, layered architecture:

### 1. UI Layer
Responsible for user interaction and screen navigation.
- `MainActivity` – Dashboard and SOS controls  
- `LoginActivity` – User authentication  
- `SafetyFragment` – Safety features interface  

### 2. Services Layer
Handles all background and emergency-related operations.
- `EmergencyService` – Manages SOS alerts and SMS dispatch  
- `LocationTrackingService` – Continuously retrieves GPS coordinates  
- `PowerButtonService` – Detects hardware button triggers  

### 3. Data Layer
Handles persistent local data storage using SQLite.
- User credentials  
- Emergency contact list  
- Location history logs  

---

## Installation and Setup

### 1. Clone the Repository
```bash
git clone https://github.com/JAIdamodharan/SOSmate.git
```

### 2. Open in Android Studio
Import the project and allow Gradle to sync all dependencies.

### 3. Grant Required Permissions
The application requires the following permissions:

- Location (Foreground and Background)  
- SMS  
- Phone Call  
- Boot Completed  
- Internet  

### 4. Initial Configuration
- Register a user account  
- Add at least one emergency contact  
- Enable all required permissions in device settings  

---

## Usage Workflow

1. User logs into the application  
2. Emergency contacts are added and verified  
3. During an emergency:
   - Tap the SOS button **or**
   - Press the power button three times  
4. Emergency SMS with live location is sent to all contacts  
5. Real-time location tracking continues until SOS mode is disabled  

---

## Performance Considerations

- Optimized for low battery consumption during background tracking  
- Uses efficient GPS polling intervals to balance accuracy and power usage  
- Lightweight SQLite database ensures fast local data access  

---

## Security and Privacy

- All user data is stored locally using SQLite  
- Location is accessed only during safety-related operations  
- No external servers store personal data in the current version  
- Emergency SMS is sent only to user-approved contacts  

---

## Limitations

- Requires network connectivity for accurate Google Maps location links  
- SMS functionality depends on SIM availability and carrier support  
- Background services may be restricted on heavily battery-optimized devices  

---

## Future Scope

- Wearable IoT integration for hands-free SOS activation  
- Cloud-based real-time tracking and emergency monitoring  
- AI-driven predictive safety alerts based on movement patterns  
- Multilingual interface support  
- Direct integration with law enforcement and emergency response APIs  

---

## Development Team

| Name | Reg. No | VIT Mail-ID |
|------|---------|-------------|
| Jaishree Damodharan | 22MIS0115 | jaishree.damodharan2022@vitstudent.ac.in |
| Pavithraa T | 22MIS0504 | pavithraa.t2022@vitstudent.ac.in |
| G. Pavithra | 22MIS0366 | pavithra.g2022b@vitstudent.ac.in |

---

## License

This project was developed for academic and research purposes. Future enhancements, deployment, and distribution may follow institutional or project-specific guidelines.
