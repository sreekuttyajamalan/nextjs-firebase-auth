Next.js 13 + Firebase Authentication

Welcome to the Next.js 13 Firebase Authentication Project! 🎉

This project demonstrates a modern authentication system built with Next.js 13 (App Router) and Firebase Authentication. Users can register, log in, and log out with email/password authentication. It’s designed with reusable components, hooks, and context, making it clean, scalable, and maintainable.

Features

Email/password registration and login

Form validation for email, password, and full name

Global authentication state using React Context

Custom hook useAuth for easy access to auth state

Protected home page with personalized greeting and logout

Clean and responsive UI with Tailwind CSS

Scalable project structure for future features

Project Structure
/app
  page.tsx          # Login page wrapper
  home/page.tsx     # Home page wrapper

/components
  LoginForm.tsx     # Login & registration form UI
  HomePage.tsx      # Home page UI with logout

/hooks
  useAuth.ts        # Custom hook for auth state consumption

/lib
  firebase.ts       # Firebase initialization

/context
  AuthContext.tsx   # Provides global auth state


Why this structure?

Separation of concerns: UI in components, logic in hooks/context

Reusability: Components and hooks are modular

Scalable: Easy to add new pages, features, or auth flows

Maintainable: Small, readable files make debugging and testing easier

Getting Started

Follow these steps to run the project locally:

1. Clone the repository
git clone https://github.com/sreekuttyajamalan/nextjs-firebase-auth.git
cd nextjs-firebase-auth


2. Install dependencies
npm install
# or
yarn

3. Configure Firebase

Go to Firebase Console

Create a new project

Enable Email/Password Authentication

Add your Firebase config keys to a .env.local file:

NEXT_PUBLIC_FIREBASE_API_KEY=your_api_key
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=your_project.firebaseapp.com
NEXT_PUBLIC_FIREBASE_PROJECT_ID=your_project_id
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=your_project.appspot.com
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=your_messaging_sender_id
NEXT_PUBLIC_FIREBASE_APP_ID=your_app_id

4. Run the development server
npm run dev
# or
yarn dev


Open http://localhost:3000
 in your browser.

How It Works

LoginForm.tsx handles both login and registration with validation.

AuthContext.tsx manages the global authentication state.

useAuth.ts is a custom hook for easy access to auth state in components.

HomePage.tsx displays a personalized greeting and logout button.

Routing is protected: users must log in to access the home page.

Usage
Registration

Switch to Register mode.

Enter full name, email, and password.

Click Register.

Login

Enter email and password.

Click Login.

Logout

Click Logout on the home page to end your session.

Technologies Used

Next.js 13
 (App Router)

React 18

Firebase Authentication

Tailwind CSS

TypeScript

Advantages

Clean & maintainable: Modular, small files

Reusable components & hooks

Scalable: Easy to add new pages or auth flows

User-friendly UI: Responsive and simple

Contributing

Contributions are welcome!

Fork the repo

Create a branch (git checkout -b feature/new-feature)

Make your changes

Commit (git commit -m "Add feature")

Push (git push origin feature/new-feature)

Open a pull request

License

This project is licensed under MIT License – see the LICENSE
 file for details.
