
<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0B1220,50:F97316,100:14B8A6&height=225&section=header&text=Melaka%20Wanderlust&fontSize=48&fontColor=FFFFFF&animation=fadeIn&fontAlignY=39&desc=Explore%20%7C%20Discover%20%7C%20Plan%20Your%20Journey&descAlignY=61&descSize=18" alt="Melaka Wanderlust" />

<br/>

<img src="melaka_wanderlust/lib/images/logo.png" alt="Melaka Wanderlust logo" width="120" />

### Discover the beauty of Melaka, one destination at a time.

A Flutter-powered tourism discovery and travel-planning application designed to help visitors explore attractions, save favorite destinations, and organize personalized itineraries around Melaka, Malaysia.

<br/>

![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)
![Dart](https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-DD2C00?style=for-the-badge&logo=firebase&logoColor=white)
![Google Maps](https://img.shields.io/badge/Google%20Maps-4285F4?style=for-the-badge&logo=googlemaps&logoColor=white)

<br/>

![Project Type](https://img.shields.io/badge/Project-University%20Team%20Project-F97316?style=flat-square)
![Platform](https://img.shields.io/badge/Platform-Flutter%20Mobile-14B8A6?style=flat-square)
![Location](https://img.shields.io/badge/Location-Melaka%2C%20Malaysia-2563EB?style=flat-square)

<br/>

[Overview](#-project-overview) •
[Features](#-key-features) •
[Tech Stack](#-technology-stack) •
[Installation](#-getting-started) •
[Contributions](#-my-contributions)

</div>

---

## 🌍 Project Overview

**Melaka Wanderlust** is a mobile tourism application developed as a university team project at **Universiti Teknikal Malaysia Melaka (UTeM)**.

The application aims to make exploring Melaka easier by combining destination discovery, location-based travel planning, budget filtering, and personalized itineraries within one mobile platform.

Instead of switching between multiple apps to research attractions, compare destinations, and plan a route, users can explore relevant places and organize their travel plans using a connected mobile experience.

### 🎯 Project Objectives

- Make tourist destinations in Melaka easier to discover.
- Help travelers choose attractions based on interests and budgets.
- Provide location-aware itinerary planning.
- Allow users to save and organize favorite destinations.
- Offer useful travel information, ratings, and local advice.

---

## ✨ Key Features

### 🗺️ 1. Discover Melaka

Explore destinations across different categories:

- 🏖️ Beaches
- 🏛️ Historical sites
- 🎡 Tourist attractions
- 🍽️ Restaurants
- 🏨 Hotels

Browse destination information and discover places of interest throughout Melaka.

### 📍 2. Interactive Maps & Itinerary Planning

Create an itinerary using selected destinations and Google Maps integration.

The itinerary module supports:

- Accessing the user's current location with permission
- Displaying selected destinations as map markers
- Ordering destinations by distance from the current location
- Retrieving estimated travel times
- Displaying route segments on the map
- Manually rearranging the order of itinerary stops

The location-based ordering uses distance calculations rather than a full route-optimization algorithm.

### ❤️ 3. Personal Wishlist

Keep favorite places organized in a personal wishlist.

Users can:

- Save destinations for future visits
- View their saved places
- Use wishlist destinations to generate an itinerary

### 💰 4. Budget & Category Filtering

Find attractions that match travel preferences.

Filtering includes:

- Minimum and maximum budget selection
- Destination categories
- Estimated attraction price information
- Results based on selected preferences

### ⭐ 5. Ratings & Reviews

Explore visitor feedback about destinations.

The project includes features for submitting and viewing destination ratings and written reviews, with Firebase Firestore used for storing review data.

### 🔐 6. Authentication & User Profiles

Firebase-based account functionality supports:

- Email and password authentication
- Account registration
- Password recovery
- User profile features

### 🧳 7. Travel Tips & Local Advice

Access useful travel information, including:

- General travel tips
- Local advice
- English and Malay travel guidance
- Tourism promotions

---

## 🛠️ Technology Stack

<div align="center">

### Mobile Development

<img src="https://skillicons.dev/icons?i=flutter,dart&theme=dark&perline=5" alt="Flutter and Dart" />

### Backend & Data

<img src="https://skillicons.dev/icons?i=firebase&theme=dark" alt="Firebase" />

### Developer Tools

<img src="https://skillicons.dev/icons?i=androidstudio,vscode,git,github&theme=dark&perline=4" alt="Developer tools" />

</div>

### Core Technologies

| Technology | Purpose |
|---|---|
| Flutter & Dart | Mobile interface and application logic |
| Firebase Authentication | Account registration and login |
| Cloud Firestore | User, wishlist, and review-related data |
| Firebase Storage | Cloud storage integration |
| Google Maps Flutter | Interactive maps and destination markers |
| Google Maps Directions API | Route and travel-time requests |
| Geolocator | Device location and distance calculations |
| Provider | Application state management |
| SharedPreferences | Local preference storage |

**Additional Flutter packages:** `permission_handler`, `flutter_rating_bar`, `image_picker`, `url_launcher`, `intl`, and `http`.

---

## 🧭 How the Travel Planning Flow Works

```text
          Open Melaka Wanderlust
                     |
                     v
             Explore Destinations
                     |
                     v
           View Destination Details
                     |
                     v
           Add Places to Wishlist
                     |
                     v
              Open My Wishlist
                     |
                     v
             Generate Itinerary
                     |
                     v
          Request Location Access
                     |
                     v
          Order Destinations by Distance
                     |
                     v
            Display Google Maps Route
                     |
                     v
          Review Times & Reorder Stops
```

The itinerary brings together wishlist data, geographic coordinates, and map directions to help users organize their selected destinations.

---

## 📂 Project Structure

```text
MelakaWanderlust/
│
└── melaka_wanderlust/
    │
    ├── android/
    ├── ios/
    ├── assets/
    │
    ├── lib/
    │   ├── components/
    │   ├── firebase/
    │   ├── icons/
    │   ├── images/
    │   ├── maps/
    │   ├── models/
    │   ├── pages/
    │   ├── tab/
    │   ├── tiles/
    │   │
    │   ├── firebase_options.dart
    │   └── main.dart
    │
    ├── test/
    └── pubspec.yaml
```

### Key Source Files

- `lib/pages/home.dart` — Home screen and destination navigation
- `lib/pages/itinerary.dart` — Maps, routes, and itinerary planning
- `lib/pages/filter.dart` — Budget and category filtering
- `lib/pages/wishlist.dart` — Saved destinations
- `lib/pages/place_detail.dart` — Destination information
- `lib/pages/review.dart` — Ratings and reviews
- `lib/pages/tips_and_advice.dart` — Travel guidance
- `lib/firebase/` — Firebase authentication integration

---

## 🚀 Getting Started

This repository contains the university project source code. A fresh installation may require dependency fixes and separate Firebase/Google Maps configuration before the application can run successfully.

### Prerequisites

- Flutter SDK with a compatible Dart version
- Android Studio or VS Code
- Android emulator or physical Android device
- Firebase project
- Google Maps Platform configuration

### 1. Clone the Repository

```bash
git clone https://github.com/salah-ayash/MelakaWanderlust.git

cd MelakaWanderlust/melaka_wanderlust
```

### 2. Check the Dependencies

Review `pubspec.yaml` and resolve any duplicate or incorrectly placed dependency entries before installing packages.

Then run:

```bash
flutter pub get
```

### 3. Configure Firebase

Connect the application to your own Firebase project.

Enable the Firebase services required by the features you intend to use, such as:

- Firebase Authentication
- Cloud Firestore
- Firebase Storage

Generate the appropriate FlutterFire configuration for your own Firebase project.

### 4. Configure Google Maps

Set up the required Google Maps Platform APIs and credentials for your development environment.

Apply appropriate API key restrictions and avoid committing unrestricted credentials or sensitive service-account keys to the repository.

### 5. Run the Application

After completing the configuration and resolving any compatibility issues:

```bash
flutter devices

flutter run
```

> **Note:** This is an academic project repository, not a published production application. The current source has not been verified as a clean build on a new machine.

---

## 👨‍💻 My Contributions

**Contributor: [Salah Ayash](https://github.com/salah-ayash)**

Melaka Wanderlust was developed collaboratively as a university team project.

My work focused particularly on location-aware travel planning and supporting mobile application features.

### Main Contributions

**Google Maps & Itinerary Planning**
- Integrated location-based itinerary functionality.
- Worked with Google Maps markers and route display.
- Implemented distance-based ordering for selected destinations.
- Supported travel-time calculations and itinerary stop reordering.

**Travel Planning Features**
- Worked on the wishlist-to-itinerary experience.
- Contributed to destination filtering and budget-related functionality.
- Supported travel information and navigation flows.

**Flutter Development**
- Developed and integrated mobile UI functionality.
- Worked with application state, navigation, and external APIs.
- Contributed to testing and improving the mobile user experience.

### Team Project Acknowledgment

The overall application—including destination discovery, user accounts, reviews, Firebase integration, and other modules—was a collaborative effort.

This repository showcases the team project and documents my personal contributions without claiming exclusive ownership of all features.

---

## 📚 Academic Context

**Project:** Melaka Wanderlust  
**Institution:** Universiti Teknikal Malaysia Melaka (UTeM)  
**Project Type:** University Group Project  
**Field:** Mobile Application Development / Tourism Technology  

The project demonstrates the practical use of mobile development, cloud-backed application features, geolocation, and mapping APIs to address real-world travel-planning needs.

---

## 🔒 Security & Configuration Notes

Before deploying or distributing the application:

- Replace and restrict any previously exposed Google Maps API keys.
- Avoid embedding unrestricted API keys directly in public source files.
- Review Firebase Authentication and Firestore security rules.
- Use appropriate permissions for location access.
- Validate dependencies and platform compatibility.
- Review sensitive configuration before publishing builds.

Historical credentials should be treated as exposed if they have been committed to a public repository.

---

## 🤝 Project Credits

Melaka Wanderlust was created through collaborative university teamwork.

Special appreciation goes to the project team for their contributions to application design, development, integration, and testing.

<div align="center">

### Developed as a university team project

**Contributor: Salah Ayash**

[![GitHub](https://img.shields.io/badge/GitHub-salah--ayash-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/salah-ayash)

<br/>

**Explore Melaka. Discover More. Plan Better.** 🌍

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:14B8A6,50:F97316,100:0B1220&height=110&section=footer" alt="Melaka Wanderlust footer" />

</div>
