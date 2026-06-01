Philippine Bird Sounds Repository

A mobile application for exploring and identifying Philippine bird species through their sounds and visual characteristics.

---

## 📱 About The Project

The **Philippine Bird Sounds Repository** is an educational mobile application developed as a school project. It serves as a reference tool for users who want to learn about bird species found in the Philippines — allowing them to browse bird information, listen to authentic bird calls, and visually identify birds through high-quality images.

> 💡 **Use Case Example:** You hear a bird sound outside but don't know what bird it is. Or you see an eagle in a photo but don't know what it sounds like. This app bridges that gap — connecting visuals and sounds to help you identify Philippine birds.

---

## ✨ Features

- 🔐 **User Authentication** — Secure sign up and login system powered by Firebase
- 🏠 **Homepage with Search** — Browse and search through the bird species list
- ➕ **Add New Bird** — Logged-in users can contribute new bird entries to the repository
- 👁️ **Bird Detail View** — View bird image, name, and detailed information
- 🔊 **Play Bird Sound** — Listen to the authentic sound/call of each bird species
- ✏️ **Edit Bird Entry** — Users can edit bird entries they have added
- 👤 **Profile Management** — View and edit your profile information and profile picture
- 🔒 **Change Password** — Update your account password
- 📞 **Contact Support** — Reach out to the developers for concerns or feedback
- ℹ️ **About Section** — Learn more about the app and its developers

---

## 🔄 App Flow

```
Open App
   │
   ▼
Login Screen ──────► Sign Up Screen
   │                      │
   │◄─────────────────────┘
   │  (login with new account)
   ▼
Homepage
   ├── Search Bar (top) — search bird by name
   ├── Add New Bird Button — add a new bird entry
   └── Bird List
         └── 👁️ View Button
               └── Bird Detail Screen
                     ├── Bird Image
                     ├── Bird Name & Information
                     └── 🔊 Play Sound Button

Menu / Navigation
   ├── Profile Screen
   │     └── Edit Profile
   ├── Change Password
   ├── Contact Support
   └── About
```

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| **React Native** | Mobile application framework |
| **Expo** | Development toolchain and build system |
| **TypeScript** | Typed JavaScript for better code reliability |
| **Expo Router** | File-based navigation/routing |
| **Firebase** | User authentication and backend database |
| **EAS (Expo Application Services)** | App building and deployment |

---

## 📂 Project Structure

```
BIRDSOUNDREPO/
├── app/
│   ├── (tabs)/                  # Tab navigation screens
│   │   ├── _layout.tsx
│   │   ├── explore.tsx
│   │   └── index.tsx
│   ├── data/
│   │   └── birds.ts             # Pre-loaded bird species data
│   ├── Menu/                    # Menu screens
│   │   ├── AboutScreen.tsx
│   │   ├── Changepass.tsx
│   │   ├── ContactSupport.tsx
│   │   ├── DeveloperSection.tsx
│   │   ├── EditProfile.tsx
│   │   └── ProfileScreen.tsx
│   ├── _layout.tsx
│   ├── AddBirdScreen.tsx        # Add new bird entry
│   ├── BirdDetailScreen.tsx     # Bird detail with sound player
│   ├── EditBirdScreen.tsx       # Edit bird entry
│   ├── Homepage.tsx             # Main homepage with search & bird list
│   ├── Loginscreen.tsx          # Login and sign up
│   └── modal.tsx
├── assets/
│   └── images/
│       ├── birdimages/          # Bird photo assets
│       └── birdsounds/          # Bird audio assets (.mp3, .wav, .m4a)
├── components/                  # Reusable UI components
├── config/
│   └── firebaseConfig.js        # Firebase configuration
├── constants/
│   └── theme.ts                 # App theme and color constants
├── hooks/                       # Custom React hooks
├── app.json                     # Expo app configuration
├── eas.json                     # EAS build configuration
└── package.json                 # Project dependencies
```

---

## 🚀 Getting Started

### Prerequisites

Make sure you have the following installed:

- [Node.js](https://nodejs.org/) (v22.20.0 or higher)
- [Expo CLI](https://docs.expo.dev/get-started/installation/)
- Android Studio (for Android emulator) or Xcode (for iOS simulator)
- Expo Go app on your physical device (optional)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/ReyFrancisS/birdsound.git
   ```

2. **Navigate to the project directory**
   ```bash
   cd birdsound
   ```

3. **Install dependencies**
   ```bash
   npm install
   ```

4. **Start the development server**
   ```bash
   npx expo start
   ```

5. **Run on your device**
   ```bash
   # Android
   npx expo run:android

   # iOS
   npx expo run:ios
   ```
   Or scan the QR code in the terminal using the **Expo Go** app on your phone.

---

## 📖 How To Use

1. **Sign Up & Login**
   - Open the app and tap **Sign Up** to create a new account
   - Log in using your registered credentials

2. **Browse Bird Species**
   - On the homepage, scroll through the list of Philippine birds
   - Use the **search bar** at the top to find a specific bird by name

3. **View Bird Details**
   - Tap the **eye icon** (👁️) beside any bird in the list
   - View the bird's image, name, and information
   - Tap **Play Sound** to hear the bird's authentic call

4. **Add a New Bird**
   - On the homepage, tap the **Add New Bird** button
   - Fill in the bird's details and submit

5. **Edit a Bird Entry**
   - You can edit birds that you personally added
   - Note: Pre-loaded birds in the system cannot be permanently overwritten (see Known Issues)

6. **Manage Your Profile**
   - Access the menu and go to **Profile**
   - Edit your name, profile picture, or change your password

---

## 👥 Development Team

| Name | Role |
|---|---|
| Rey Francis S. | Lead Developer — Full system development |
| [Teammate 2] | Wireframe / UI Design |
| [Teammate 3] | Data Collection (Bird species data) |

---

## 🐛 Known Issues

- **Pre-loaded bird duplication on edit** — When a user attempts to edit a pre-loaded (default) bird entry, the original entry is not overwritten. Instead, a duplicate is created, resulting in two entries: the original unchanged bird and the edited version. This is a known bug. User-added birds are not affected by this issue.

---

## 🔮 Future Updates

- [ ] Fix duplication bug for pre-loaded bird entries
- [ ] Admin role — restrict editing/deleting of default bird list to admins only
- [ ] Offline mode — browse birds without internet connection
- [ ] Bird call recording — record a sound and compare it to the database
- [ ] Gamification — achievements and badges for exploration
- [ ] Multi-language support (Filipino / English)
- [ ] AR bird identification

---

## 📸 Screenshots

> <img width="444" height="816" alt="Screenshot 2026-06-01 174223" src="https://github.com/user-attachments/assets/ea9f419d-6c37-457a-b83b-3e31b1bf0f94" />
> <img width="440" height="813" alt="Screenshot 2026-06-01 174308" src="https://github.com/user-attachments/assets/eaed173f-906e-4837-9d98-43f371b8f661" />
> <img width="440" height="891" alt="Screenshot 2026-06-01 174736" src="https://github.com/user-attachments/assets/b130d58b-f449-4885-a4ba-42e1a46b8d6c" />
> <img width="438" height="933" alt="Screenshot 2026-06-01 174404" src="https://github.com/user-attachments/assets/5647cada-fce3-48fc-8487-980ecaf407f5" />
> <img width="441" height="843" alt="Screenshot 2026-06-01 174503" src="https://github.com/user-attachments/assets/0ad5cee3-7da9-4687-8d5f-79f5063ad9f7" />
> <img width="441" height="879" alt="Screenshot 2026-06-01 174641" src="https://github.com/user-attachments/assets/b34d1da3-196d-49ea-bff1-95cef61adc92" />
> <img width="441" height="928" alt="Screenshot 2026-06-01 174559" src="https://github.com/user-attachments/assets/40bd1f8c-70b3-4908-b2a1-88fb5c064a81" />


---

## 📝 License

This project was developed as an academic requirement. All bird sounds and images used are for educational purposes only.

---

## 📞 Contact

- **GitHub:** [ReyFrancisS](https://github.com/ReyFrancisS)
- **Email:** sisonreyfrancis19@gmail.com

---

*Made with ❤️ for Philippine Bird Conservation — School Project*
