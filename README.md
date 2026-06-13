# Geomark: Landmark-Based Business Discovery System 

**Geomark** is a custom-built web application designed to bridge the digital visibility gap for informal Small and Medium Enterprises (SMEs) in East Africa. By utilizing a landmark-based navigation approach, this platform allows businesses without formal street addresses in Nairobi, Dar es Salaam, and Kampala to establish an accurate, discoverable online presence.

## The Problem & Solution
Standard global mapping applications rely on Western-style grid systems and gazetted street names, which often exclude informal businesses in East Africa. 

**Geomark** solves this by shifting the focus from street addresses to **familiar physical landmarks**. SME owners can drop a pin relative to a well-known local landmark, allowing consumers to easily search for, discover, and navigate to local services using natural, community-based wayfinding.

## Key Features
* **Interactive Mapbox Integration:** Modern, dark-themed interactive map for pinpointing business locations.
* **Landmark-Based Proximity Search:** Links businesses to coordinates of known landmarks.
* **Secure Authentication:** Encrypted passwords and 6-digit email verification via PHPMailer.
* **Role-Based Dashboards:** * **Consumers:** Open-access map search.
    * **SME Owners:** Dedicated portal to manage business profiles, update operational hours, and pin locations.
    * **System Administrators:** Secure panel to verify businesses, manage users, and view system analytics.
* **Responsive UI:** Clean, minimalist, and accessible design optimized for varying network conditions.

## Technology Stack
* **Frontend:** HTML5, CSS3 (Custom Variables, Flexbox/Grid), JavaScript (ES6)
* **Backend:** PHP (PDO for secure database interactions)
* **Database:** MySQL (Relational Schema with Foreign Key constraints)
* **APIs & Libraries:** Mapbox GL JS (Mapping), PHPMailer (SMTP Email Auth)
* **Development Environment:** XAMPP / VS Code

## 📂 Project Structure
```text
geomark/
├── css/
│   └── style.css            # Advanced styling and animations
├── js/
│   └── script.js            # Frontend validation logic
├── PHPMailer/               # Email authentication library
│   └── src/
├── config.php               # Database connection settings
├── index.php                # Consumer landing page & map search
├── login.php                # Authentication gateway
├── register.php             # SME registration and email trigger
├── verify.php               # 6-digit code verification handler
├── reset_password.php       # Password recovery logic
├── sme_dashboard.php        # SME portal and Mapbox pin-dropping
├── save_location.php        # Backend handler for map coordinates
├── admin_dashboard.php      # Administrative control panel
└── README.md                # Project documentation
