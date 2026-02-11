# SOSMate - Personal Safety Application

SOSMate is an Android-based smart safety application designed to provide immediate emergency assistance and real-time protection. The application focuses on personal security, particularly for women and vulnerable individuals, by enabling rapid distress signaling and location sharing.

## Features

* 
**One-Touch SOS Activation**: Trigger emergency alerts instantly via a dedicated SOS button on the main dashboard.


* 
**Power Button Trigger**: Discreetly initiate emergency alerts by pressing the power button three consecutive times.


* 
**Automatic Emergency SMS**: Automatically sends an SMS containing a Google Maps location link to all pre-registered emergency contacts when SOS is triggered.


* 
**Real-Time Location Tracking**: Continuously monitors and updates the user's live location using Google Play Services.


* 
**Fake Call Simulation**: Allows users to simulate an incoming call to discreetly exit potentially unsafe situations.


* 
**Background Services**: Includes features like auto-start on device reboot to ensure uninterrupted safety monitoring.


* 
**Location History**: Maintains a log of previously recorded locations with timestamps for reference.


* 
**Emergency Contact Management**: Allows users to add, edit, and delete emergency contacts through a dedicated interface.



## Technical Stack

* 
**Operating System**: Android 8.0 (Oreo) and above.


* 
**Language**: Java for core logic and XML for front-end layout design.


* 
**Development Environment**: Android Studio with Gradle Build System.


* 
**Database**: SQLite for local storage of user credentials, emergency contacts, and location records.


* 
**APIs**: Google Play Services (Location API) and Google Maps API.


* 
**Libraries**: AndroidX and Material Design Libraries for UI/UX consistency.



## Architecture

The application follows a modular architecture that separates the user interface, background services, and data management.

* 
**UI Layer**: Manages user interactions through activities and fragments like `MainActivity`, `LoginActivity`, and `SafetyFragment`.


* 
**Services Layer**: Handles background tasks including `EmergencyService` for alerts, `LocationTrackingService` for GPS updates, and `PowerButtonService` for hardware triggers.


* 
**Data Layer**: Manages persistent storage using an SQLite database with tables for users, contacts, and location history.



## Installation and Setup

1. **Clone the Repository**:
```bash
git clone https://github.com/JAIdamodharan/SOSmate.git

```


2. 
**Open in Android Studio**: Import the project and allow Gradle to sync dependencies.


3. 
**Permissions**: Ensure the application is granted permissions for Location, SMS, and Phone calls to function correctly.


4. 
**Configuration**: Register an account and add at least one emergency contact to enable SOS features.



## Team Members

* Jaishree Damodharan (22MIS0115) 


* Pavithraa T (22MIS0504) 


* G. Pavithra (22MIS0366) 



## Future Scope

* Integration with wearable IoT devices for hands-free SOS triggering.


* Cloud-based data synchronization for real-time tracking and analytics.


* AI-driven predictive alerts based on movement pattern analysis.


* Multilingual interface support for improved accessibility.


* Integration with Law Enforcement APIs for direct police notification.
