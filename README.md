# 🔐 Secure Password Generator

A powerful and user-friendly **React-based password generator** with advanced features including strength assessment, password history, favorites, and local storage persistence.

## ✨ Features

- **🔑 Smart Password Generation**: Generate secure passwords with customizable options
  - Uppercase letters (A-Z)
  - Lowercase letters (a-z)
  - Numbers (0-9)
  - Special symbols (#@$%^&* etc.)
  
- **📊 Password Strength Meter**: Real-time strength assessment (Weak/Medium/Strong)
  - Considers length and character variety
  - Color-coded strength indicator

- **📜 History Management**: Automatically tracks last 20 generated passwords
  - View all previously generated passwords
  - Search functionality to find passwords by name or content
  - Timestamp for each password

- **⭐ Favorites System**: Save important passwords as favorites
  - Quick access to frequently used passwords
  - One-click favorites toggle

- **📋 Copy to Clipboard**: One-click password copying with visual feedback
  - Eye icon to toggle password visibility
  - Copy confirmation notification

- **💾 Local Storage**: All data persists in your browser
  - No server uploads - your passwords stay private
  - Settings automatically saved

- **⚙️ Settings Panel**: Customize your experience
  - Auto-copy generated passwords option
  - Toggle additional preferences

- **🔔 Notifications**: Real-time feedback for user actions
  - Copy confirmations
  - Generation success messages

## 📸 Screenshots

### Main Interface
![App Preview](screenshots/app-preview.png)

### Password History
![History View](screenshots/history-view.png)

## 🛠️ Tech Stack

- **React 18+**: UI framework
- **React Icons**: Beautiful icon library (FontAwesome)
- **Crypto API**: Secure random number generation
- **CSS3**: Modern styling with animations
- **LocalStorage API**: Client-side data persistence

## 🚀 Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/vpraveenk1202/password-generator.git
   cd password-generator
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm start
   ```
   The app will open at `http://localhost:3000` in your browser.

## 📖 How to Use

1. **Set Password Length**: Use the slider to choose length (default: 12 characters)
2. **Select Character Types**: Toggle uppercase, lowercase, numbers, and symbols
3. **Add Description** (Optional): Name your password (e.g., "Gmail", "Facebook")
4. **Generate Password**: Click the "Generate Password" button
5. **Copy**: Click the copy icon or use the copy button
6. **Save to Favorites**: Click the star icon to bookmark important passwords
7. **Search History**: Use the search bar to find previous passwords
8. **Access Settings**: Click gear icon to enable auto-copy feature

## 💡 Code Overview

### Key Components in App.js:

- **Password Generation**: Uses Web Crypto API (`crypto.getRandomValues()`) for cryptographically secure random generation
- **Strength Calculation**: Analyzes length and character types to determine password strength
- **Local Storage Management**: Saves history, favorites, and settings to browser storage
- **Performance Optimization**: Uses `useMemo` and `useCallback` hooks to prevent unnecessary re-renders
- **User Notifications**: Toast-style notifications for user actions

### Algorithm Complexity:
- **Password Generation**: O(n) - where n is password length
- **Strength Calculation**: O(n) - scans password once
- **History Search**: O(m) - where m is number of stored passwords

## 🔒 Security Features

- **Client-Side Only**: All operations happen in your browser - no data sent to servers
- **Cryptographically Secure**: Uses `window.crypto.getRandomValues()` for true randomness
- **No External Dependencies for Encryption**: Minimal attack surface

## 📦 Scripts

```bash
npm start      # Start development server
npm run build  # Create production build
npm test       # Run tests
npm run eject  # Eject from Create React App (one-way operation)
```

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Fork the repository
- Create a feature branch (`git checkout -b feature/AmazingFeature`)
- Commit changes (`git commit -m 'Add some AmazingFeature'`)
- Push to the branch (`git push origin feature/AmazingFeature`)
- Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👨‍💻 Author

Created by **Praveen Kumar V**

## 🐛 Issues & Feedback

Found a bug? Have a suggestion? Please open an issue on GitHub!

---

**Built with ❤️ and React** | Made to keep your passwords secure and easily accessible
