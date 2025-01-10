Sure! Here's a README template based on the one you provided, but with your changes applied:

---

# Salinaka | E-commerce React App

A simple e-commerce application built with React JS, TypeScript, and Firebase. This app allows users to browse products, register accounts, and perform various actions such as product CRUD operations. It's designed to be lightweight and easy to deploy on Firebase.

![Firebase Deploy](https://github.com/jgudo/ecommerce-react/workflows/Firebase%20Deploy/badge.svg)

### [Live Demo](https://salinaka-ecommerce.web.app/)

![Salinaka screenshot](https://raw.githubusercontent.com/jgudo/ecommerce-react/master/static/screeny1.png)
![Salinaka screenshot](https://raw.githubusercontent.com/jgudo/ecommerce-react/master/static/screeny2.png)
![Salinaka screenshot](https://raw.githubusercontent.com/jgudo/ecommerce-react/master/static/screeny3.png)
![Salinaka screenshot](https://raw.githubusercontent.com/jgudo/ecommerce-react/master/static/screeny7.png)

## Run Locally

### 1. Install Dependencies
To begin, install the necessary dependencies using yarn:

```bash
$ yarn install
```

### 2. Set Up Firebase

Create a new Firebase project by logging into your Google account and visiting [Firebase Console](https://console.firebase.google.com/u/0/).

Afterward, create a `.env` file and add the following Firebase configuration variables:

```bash
// SAMPLE CONFIG .env, you should use the actual Firebase project details from your Firebase settings

VITE_FIREBASE_API_KEY=AIzaKJgkjhSdfSgkjhdkKJdkjowf
VITE_FIREBASE_AUTH_DOMAIN=yourauthdomain.firebaseapp.com
VITE_FIREBASE_DB_URL=https://yourdburl.firebaseio.com
VITE_FIREBASE_PROJECT_ID=yourproject-id
VITE_FIREBASE_STORAGE_BUCKET=yourstoragebucket.appspot.com
VITE_FIREBASE_MSG_SENDER_ID=43597918523958
VITE_FIREBASE_APP_ID=234598789798798fg3-034
```

### 3. Firebase Database Setup

Go to Firebase Console, create a **Cloud Firestore Database**, and set the security rules to test mode for now.

### 4. Start Development Server

Run the following command to start the local development server:

```bash
$ yarn dev
```

---

## Build the Project

To build the production version of the app, run the following:

```bash
$ yarn build
```

## Admin Features and CRUD Operations

1. Navigate to `/signup` on your app.
2. Register an account for yourself.
3. In the Firebase Firestore console, locate the `users` collection and edit the newly created user. Change their role from `USER` to `ADMIN`.
4. Reload or sign in again to see the changes.

**Firebase Admin integration coming soon!**

## Features

* **Admin CRUD Operations**: Admins can create, read, update, and delete products.
* **Firebase Authentication**: Includes Firebase authentication for secure login and account management.
* **Provider Authentication**: Supports Firebase auth provider integrations (e.g., Google login).
* **Account Management**: Admins can manage accounts and perform CRUD operations.

---

Make sure to modify the Firebase credentials, change any branding, and add any custom functionality you've developed.
