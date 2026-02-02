# Checkmate — Smart QR-based Attendance System

A modern React application for intelligent attendance tracking with real-time engagement monitoring, face verification, and comprehensive analytics. Built with a sleek dark theme and glassmorphism design.

## 📋 Project Details
- **Repository**: [https://github.com/prajan1110/Checkmate-Smart-QR-based-Attendance-System](https://github.com/prajan1110/Checkmate-Smart-QR-based-Attendance-System)
- **Version**: 1.0.0
- **License**: MIT

## ✨ Key Features

### 🎯 **Smart Attendance Tracking**
- QR code generation and scanning for seamless check-ins
- Real-time face verification during attendance
- Automated liveness scoring based on participant engagement
- Session management with detailed analytics

### 📊 **Engagement Monitoring**
- Dynamic popup questions during sessions
- Configurable timing modes (Manual/Auto Random)
- Real-time engagement scoring and statistics
- Comprehensive participant response tracking

### 🎨 **Modern UI/UX**
- Dark theme with glassmorphism effects
- Smooth animations and transitions
- Responsive design for all devices
- Professional gradient styling

## 🛠️ Tech Stack
- **React 19** - Modern JSX with hooks
- **Vite** - Fast development and build tooling
- **html5-qrcode** - Camera-based QR scanning
- **qrcode** - QR code generation
- **CSS3** - Advanced styling with backdrop-filter and animations
- **Firebase** - Backend services for data storage and authentication

## 🔐 Credentials Setup

This project uses Firebase for backend services. To set up the credentials:

1. Create a Firebase project at [https://console.firebase.google.com/](https://console.firebase.google.com/)
2. Enable the required services (Authentication, Firestore, etc.)
3. Copy your Firebase config from the project settings
4. Create a `.env` file in the root directory with the following variables:

```env
VITE_FIREBASE_API_KEY=your_api_key_here
VITE_FIREBASE_AUTH_DOMAIN=your_project.firebaseapp.com
VITE_FIREBASE_PROJECT_ID=your_project_id
VITE_FIREBASE_STORAGE_BUCKET=your_project.appspot.com
VITE_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
VITE_FIREBASE_APP_ID=your_app_id
```

**Note**: Never commit the `.env` file to version control. The `.env.example` file is provided as a template.

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ and npm
- Modern browser with camera access
- Windows/macOS/Linux

### Installation

```bash
# Clone the repository
git clone https://github.com/prajan1110/Checkmate-Smart-QR-based-Attendance-System
cd Checkmate-Smart-QR-based-Attendance-System

# Install dependencies
npm install

# Start development server
npm run dev
```

### Access the Application
Open your browser at `http://localhost:5173` (default Vite port)

## 📱 How to Use

### For Organizers
1. **Create Session**: Enter session name and configure settings
2. **Generate QR Code**: Download and display QR for participants
3. **Manage Questions**: Add engagement questions with correct answers
4. **Configure Popups**: Set timing mode (Manual/Auto) and duration
5. **Monitor Analytics**: View real-time engagement scores and statistics

### For Participants
1. **Scan QR Code**: Use camera to scan session QR
2. **Face Verification**: Complete liveness check for attendance
3. **Answer Questions**: Respond to popup engagement questions
4. **View Confirmation**: See attendance verification with session details

## 📁 Project Structure

### Core Pages
- `src/pages/Organizer.jsx` — Complete organizer dashboard with analytics
- `src/pages/Scan.jsx` — QR scanning with face verification flow
- `src/pages/AttendanceVerified.jsx` — Success page with session details

### Components
- `src/components/Card.jsx` — Glassmorphism card component
- `src/components/Button.jsx` — Modern gradient buttons
- `src/components/Toast.jsx` — Notification system
- `src/components/EngagementPopup.jsx` — Dynamic question popups

### Hooks & Logic
- `src/hooks/useEngagementPopups.js` — Engagement system logic
- `src/App.jsx` — Main app routing and layout
- `src/App.css` — Comprehensive styling system

## 🔧 Available Scripts

```bash
npm run dev      # Start development server with hot reload
npm run build    # Create optimized production build
npm run preview  # Preview production build locally
npm run lint     # Run ESLint for code quality
```

## 🔍 Technical Implementation

### QR Code System
- **Scanning**: Advanced `html5-qrcode` integration with custom styling
- **Generation**: High-quality QR codes with download functionality
- **Verification**: Real-time validation and error handling

### Engagement System
- **Popup Management**: Configurable timing and duration controls
- **Score Calculation**: Accurate engagement metrics (correct/total questions)
- **Data Persistence**: localStorage integration for session tracking

### Face Verification
- **Liveness Detection**: Ensures real participant presence
- **Security**: Prevents attendance spoofing
- **User Experience**: Smooth verification flow with feedback

## 🎯 Current Features

### ✅ **Implemented**
- Modern dark theme with glassmorphism design
- Complete engagement popup system with timing controls
- Real-time liveness scoring and analytics
- Face verification during attendance
- Professional UI with smooth animations
- Responsive design for all devices
- Advanced QR scanning with custom styling
- Session management and statistics
- localStorage data persistence

### 🚀 **Future Enhancements**

#### Backend Integration
- RESTful API for session management
- Real-time participant tracking
- Secure token-based authentication
- Cloud data synchronization

#### Advanced Features
- TypeScript migration for better type safety
- Comprehensive test suite (Jest/Vitest)
- CI/CD pipeline with GitHub Actions
- PWA capabilities for offline use

#### Security & Performance
- Encrypted QR payloads
- Bundle optimization and lazy loading
- Enhanced accessibility (WCAG compliance)
- Advanced analytics dashboard

## 🎨 Design System

### Color Palette
- **Primary**: Gradient blues and purples
- **Background**: Dark theme with subtle patterns
- **Glass Effects**: Backdrop-filter blur with transparency
- **Accents**: Success greens, warning oranges, error reds

### Typography
- **Headings**: Bold, modern font weights
- **Body**: Clean, readable text with proper contrast
- **Interactive**: Hover states and smooth transitions

## 📊 Data Management

### localStorage Schema
```javascript
// Session data
`session_${sessionId}` // Session configuration
`questions_${sessionId}` // Question bank
`responses_${sessionId}` // Participant responses
`liveness_${sessionId}` // Engagement scores
```

### Engagement Scoring
- **Formula**: (Correct Answers / Total Questions Sent) × 100
- **Real-time**: Updates as participants respond
- **Persistent**: Stored across browser sessions

## 🤝 Contributing

We welcome contributions! Please feel free to:
- Report bugs and issues
- Suggest new features
- Submit pull requests
- Improve documentation

## 📄 License

This project is open source and available under the MIT License.

---

**Ready to use!** Run `npm install && npm run dev` to start the development server.