# 🚀 Next.js 13 + Firebase Authentication

Welcome! This is a **Next.js 13** project with **Firebase Authentication**.  
Users can **register, log in, and log out** using email/password.  
The project is **modular, scalable, and easy to maintain**, with hooks, context, and reusable components.

---

## ✨ Features

- ✅ Email/password registration and login  
- ✅ Form validation for email, password, and full name  
- ✅ Global auth state with **React Context**  
- ✅ Custom hook `useAuth` for easy auth state access  
- ✅ Protected Home page with personalized greeting and logout  
- ✅ Clean UI with **Tailwind CSS**  
- ✅ Scalable and reusable code structure  

---

## 📁 Project Structure

- **/app**
  - `page.tsx` – Login page wrapper  
  - `home/page.tsx` – Home page wrapper  

- **/components**
  - `LoginForm.tsx` – Login & registration UI  
  - `HomePage.tsx` – Home page with logout  

- **/hooks**
  - `useAuth.ts` – Custom hook for auth  

- **/lib**
  - `firebase.ts` – Firebase setup  

- **/context**
  - `AuthContext.tsx` – Global auth state  

---

## ⚡ Getting Started

### 1️⃣ Clone the repository
```bash
git clone https://github.com/sreekuttyajamalan/nextjs-firebase-auth.git
cd nextjs-firebase-auth
2️⃣ Install dependencies
bash
Copy code
npm install
# or
yarn
3️⃣ Configure Firebase
Go to Firebase Console

Create a new project

Enable Email/Password Authentication

Create a .env.local file in the root and add your credentials:

env
Copy code
NEXT_PUBLIC_FIREBASE_API_KEY=your_api_key
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=your_project.firebaseapp.com
NEXT_PUBLIC_FIREBASE_PROJECT_ID=your_project_id
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=your_project.appspot.com
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=your_messaging_sender_id
NEXT_PUBLIC_FIREBASE_APP_ID=your_app_id
4️⃣ Run the development server
bash
Copy code
npm run dev
# or
yarn dev
Open http://localhost:3000 to view the app.

📝 How It Works
LoginForm.tsx – Handles login and registration with validation

AuthContext.tsx – Manages global auth state

useAuth.ts – Custom hook to access auth state easily

HomePage.tsx – Shows personalized greeting and logout

Protected routing – Ensures users must log in to access Home page

🛠 Technologies
Next.js 13

React 18

Firebase Authentication

TypeScript

🎯 Advantages
✨ Clean and maintainable structure

♻️ Reusable components & hooks

🚀 Scalable for adding new features

🎨 User-friendly, responsive UI

🤝 Contributing
🍴 Fork the repo

🌿 Create a branch (git checkout -b feature/new-feature)

✏️ Make changes and commit

⬆️ Push (git push origin feature/new-feature)

🔀 Open a pull request

