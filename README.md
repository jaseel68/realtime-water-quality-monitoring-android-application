An IoT-based system that monitors water quality in real time using sensors and displays the data through a mobile application. Users can scan a QR code to instantly access water quality status along with a health-based conclusion.

[ Sensors ] → [ Microcontroller ] → [ Firebase Cloud ]
                                      ↓
                              [ Mobile App ]
                                      ↓
                                 [ QR Access ]


⚙️ Installation & Setup
🔹 1. Clone Repository
git clone https://github.com/your-username/your-repo.git
cd your-repo


2. Setup IoT Device (ESP8266 / ESP32)
# Install required libraries in Arduino IDE
- WiFi.h
- Firebase ESP Client
- Sensor-specific libraries

Update credentials in code:

#define WIFI_SSID "your_wifi"
#define WIFI_PASSWORD "your_password"
#define API_KEY "your_firebase_api_key"
#define DATABASE_URL "your_database_url"

Upload code to microcontroller.



🔹 3. Run Mobile App (Flutter)
# Install dependencies
flutter pub get

# Run app
flutter run


🔹 4. Firebase Setup
Create Firebase project
Enable Firestore / Realtime DB
Add Android app
Download google-services.json and place inside:
android/app/



📊 Sample Output
pH Level       : 7.2
Turbidity      : Low
TDS            : 150 ppm
Temperature    : 28°C

Status: ✅ Safe for Drinking



