# Sport Matchmaking App

## Project Overview

This mobile application is designed for university students to host and join sports games, while integrating with the university's court booking system. The app allows users to:
- Host games and specify details like sport, date, time, and court.
- Find and join games hosted by other students.
- View match details in a minimalistic interface.

## Technologies Used
- **Front-end:** React Native
- **Back-end:** Supabase
- **AI Dev Tools:** Cursor or Windsurf (for enhanced coding efficiency)

## Getting Started

1. **Set up Supabase:**
   - Create a new Supabase project and set up the necessary tables and authentication.

2. **Set up React Native Project:**
   - Initialize a new React Native project.
   - Integrate Supabase client for data operations and authentication.

3. **Implement Features:**
   - User authentication with email verification for university domains.
   - Game hosting with manual input of booking details.
   - Game browsing and joining.
   - Display match details.

4. **Test and Deploy:**
   - Test the app on simulators or devices.
   - Deploy for testing within the university or prepare for app store submission.

## Dependencies
- [React Native](https://reactnative.dev/)
- [Supabase JavaScript Client](https://supabase.com/docs/reference/javascript)
- [Expo](https://expo.dev/) (optional for easier development)

## Instructions for Users
1. **Book a Court:**
   - Visit the university's booking system at [bsu.uitm.edu.my](https://bsu.uitm.edu.my/) to book a court.
   - Enter the booking details when hosting a game in the app.

2. **Host a Game:**
   - Log in to the app.
   - Navigate to the "Host Game" screen and fill in the game details, including the booking information.

3. **Join a Game:**
   - Log in to the app.
   - Browse the list of available games and join one by clicking the "Join" button.

4. **View Match Details:**
   - From the game list or directly from a game's page, view detailed information about the game and its participants.

# Project Roadmap

## 1. Back-End Setup with Supabase

### Steps:
1. **Create a Supabase Project:**
   - Sign up for a Supabase account.
   - Create a new project.

2. **Set Up Tables:**
   - **Users Table:**
     - Columns: `id` (primary key), `email`, `name`, `password_hash`, etc.
     - Use Supabase's built-in authentication to manage user accounts.
   - **Games Table:**
     - Columns: `id` (primary key), `host_id` (foreign key to users), `sport`, `date`, `time`, `court`, `description`, etc.
     - Participants can be managed through a separate table or an array.
   - **Bookings Table:**
     - If needed, to link games to specific court bookings.
     - Columns: `game_id` (foreign key to games), `booking_id` (from university system, if available), etc.

3. **Configure Authentication:**
   - Set up email verification to ensure only university email domains can sign up.
   - Use Supabase's authentication API to handle login and signup.

## 2. Front-End Development with React Native

### Steps:
1. **Initialize React Native Project:**
   - Use `npx react-native init MyApp` or create an Expo project.

2. **Set Up Supabase Client:**
   - Install the Supabase JavaScript client.
   - Configure the client with your Supabase project URL and key.

3. **Implement User Authentication:**
   - Create screens for login and signup using Supabase's authentication methods.
   - Handle email verification for university email domains.

4. **Develop Game Hosting Feature:**
   - Create a screen where users can input game details, including booking information from the university's system.
   - Validate input formats for date and time.

5. **Develop Game Browsing and Joining Features:**
   - Display a list of available games.
   - Allow users to join games by adding their user ID to the game's participants list.

6. **Display Match Details:**
   - Create a screen to show detailed information about a game, including participants.

## 3. Integration with University's Booking System

### Approach:
- Since direct API integration is not possible, users must manually book courts through the university's system and input those details when hosting a game.
- The app will not check for booking availability; users are responsible for ensuring their bookings are valid and conflict-free.

### Steps:
1. **Provide Instructions:**
   - In the app, provide clear instructions on how to book a court through the university's system.
   - Include a link to the university's booking system.

2. **Input Validation:**
   - When hosting a game, validate the input fields for date, time, and court to ensure they are in the correct format.
   - Optionally, implement basic checks to ensure the date and time are in the future.

## 4. Testing and Deployment

### Steps:
1. **Test on Simulators/Devices:**
   - Test the app on both Android and iOS simulators or physical devices.
   - Ensure all features work as expected, including authentication, game hosting, browsing, joining, and displaying details.

2. **Deploy the App:**
   - For testing within the university, provide installation instructions or host the app on a local server.
   - If desired, prepare the app for submission to app stores (Google Play Store, Apple App Store).

This project aims to provide a seamless experience for university students to organize and participate in sports games, leveraging the university's existing infrastructure for court bookings.