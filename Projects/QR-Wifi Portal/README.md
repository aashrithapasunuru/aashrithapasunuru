## QR Code WIFI Captive Portal Simulation

A Flask-based WIFI Captive Portal simulation that demonstrates how public WIFI onboarding systems operate
operate in airports, hotels, cafes and other public venues. 

Users scan a QR code to access a branded WIFI portal, provide optional identification details, grant location
access and connect to a simulated WIFI network. The application captures connection metadata, generate a unique
WIFI session ID, and logs user activity for analysis. 

This project was developed to explore web  development, networking concepts, logging mechanisms and security
telemetry collection in a realistic captive portal workflow. 

# Features
- QR Code-based portal access
- Responsive airport-style captive portal interface
- username collection(optional)
- Browser geolocation integration
- Automatic wifi session ID generation
- Device type detection (Mobile, Tablet, Desktop)
- Browser and operating system identification
- User-Agent analysis
- SQLite database logging
- Session-based user tracking
- Connection success page with session details
- Grateful handling of location permission denial
- Mobile and desktop compatibility
- HTTPS support via ngrok for secure testing

  # Technologies Used
  - python
  - Flask
  - HTML5
  - CSS3
  - Javascript
  - SQLite
  - Geolocation API
  - User-Agent Parsing
  - ngrok
    
  # Workflow
  - User scans a QR code.
  - The captive portal opens in a web browser.
  - User optionally enters a name.
  - Browser requests location permission.
  - Application collects location and device information.
  - A unique WIFI session ID is generated.
  - Connection details are stored in SQLite.
  - User is redirected to a success page displaying connection information.
    
 
  # Architecture
  
    QR Code
      ↓
    Flask Web Portal
      ↓
    Geolocation API
      ↓
    Session Generation
      ↓
    SQLite Logging
      ↓
    Success Page
 
  # Logged Information
    
    The application stores
 
  - Timestamp
  - IP Address
  - Browser Information
  - Operating system
  - Device Type
  - Username
  - Generated wifi session ID
  - Latitude and Longitude Coordinates
  - User-Agent string
    
 
  # Skills Demonstrated

  **Web Development & Programming**
  - Flask web development
  - Client-server communication
  - Form processing and validation
  - Session management
  - Database integration using SQLite
  - Front-end development with HTML, CSS and Javascript
  - API interaction using the browser Geolocation API

  **Networking Concepts**
  - QR code-based access workflows
  - HTTP and HTTPS communication
  - Public WIFI onboarding processes
  - Captive portal simulation
  - Client device identification
  - IP address collection and logging
  - Network access event tracking
 
  **Cybersecurity Concepts**
  - User activity logging and monitoring
  - Security event data collection
  - User-Agent analysis
  - Browser and operating system identification
  - Geolocation-based access tracking
  - Audit trail generation
  - Collection and storage of security -revelant metadata
  - Understanding how public wifi portals gather telemetry
  - Foundations of Security Information and Event Management(SIEM) data generation
 
  **SOC Analyst Relevance**
  
  This project demonstrates several concepts commonly encountered in Security Operations Centers(SOC),
  including:
  - Log generation and analysis
  - Security event collection
  - Endpoint and device identification
  - User activity monitoring
  - Investigation of connection metadata
  - Audit trail creation
  - Understanding how network access events are recorded and monitored
    
 
  **Network Analyst Relevance**
  
  This project also helps build familiarity with:
  - Network access workflows
  - Client connectivity processes
  - Device classification
  - IP-based identification
  - Public network access architectures
  - User onboarding mechanisms
  - Connection event monitoring
    
 
  **Disclaimer**
  
    This project is intended for educational and demonstration purposes only. It simulates a captive portal workflow and does not provide actual WiFi authentication, authorization, or network access control functionality.
   
