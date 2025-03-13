# Sportea 🏆

> A university sports matchmaking mobile application

## 📱 Project Overview

Sportea is a final year computer science project aimed at creating a mobile application for sports matchmaking within a university campus. The app allows students to:

- Find sports games/matches hosted by other students
- Host games and invite participants
- Browse available games filtered by sport type
- Book courts directly through the app
- Integrate with the university's existing booking system (https://bsu.uitm.edu.my/)

## 🎯 Key Features

- **Matchmaking System**: Connect players and teams for various sports
- **Game Hosting**: Allow users to create and manage sports events
- **Court Booking Integration**: Synchronize with the university's existing booking platform
- **University-Restricted Access**: Limited to university students using their official email addresses
- **Game Roster Display**: Minimalistic interface showing match participants (similar to video game lobbies)

## 🔄 Integration with University Booking System

A core feature of Sportea is its integration with the university's existing booking system:

- Credentials for hosted games will sync with the university booking database
- Students won't need to manually use both systems separately
- Booking conflicts will be prevented through real-time synchronization
- The entire booking process will be streamlined and aligned

## 💻 Technical Stack Recommendations

### Frontend Options
- **React Native**: Recommended for cross-platform development with excellent performance and wide community support
- **Flutter**: Good alternative with a single codebase for both iOS and Android
- **Swift/Kotlin**: For native development if targeting a single platform initially

### Backend Options
- **Firebase**: Recommended for rapid development, real-time database, authentication services, and easy mobile integration
- **Supabase**: Good open-source alternative to Firebase with PostgreSQL database
- **Hostinger + Custom Backend**: More work but provides greater flexibility if custom logic is needed

### AI Development Tools
- **Cursor**: Excellent for code assistance and pair programming with AI
- **GitHub Copilot**: Seamless integration with most IDEs for code suggestions
- **Replit**: Good for quick prototyping and collaboration
- **Windsurf**: Consider for specific AI-driven features

## 🚀 Project Roadmap

1. **Planning & Research Phase**
   - Define detailed user requirements
   - Study university booking system API/integration options
   - Select final technology stack

2. **Design Phase**
   - Create wireframes and UI/UX design
   - Design database schema
   - Plan API endpoints

3. **Development Phase**
   - Implement user authentication (university email restriction)
   - Build court booking and game hosting features
   - Develop integration with university booking system
   - Create match browsing and joining functionality

4. **Testing Phase**
   - Conduct unit and integration testing
   - Perform user acceptance testing with student volunteers
   - Stress test booking system integration

5. **Deployment & Maintenance**
   - Deploy to app stores (or internal university distribution)
   - Monitor performance and gather user feedback
   - Implement improvements and fixes

## 📋 Prerequisites

- University student account
- Mobile device (iOS or Android)
- Internet connection

## 🔒 Security & Privacy

- Limited access to university email holders only
- User data protected according to university data policies
- Integration with university systems following secure protocols

## 📬 Contact

For questions or suggestions about this final year project, please contact the developer.

---

*This project is being developed as a final year computer science project.*