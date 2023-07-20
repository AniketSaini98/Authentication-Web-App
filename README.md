# Node.js Authentication System

This is a complete authentication system built with Node.js that can serve as a starter code for creating new applications. It includes features like user sign-up, sign-in, sign-out, reset password, and social authentication (Google login/signup). The system also handles encryption of passwords stored in the database and displays appropriate notifications for unmatching passwords during sign-up and incorrect passwords during sign-in. Additionally, it has a bonus feature for handling forgot passwords.

## Setup Instructions

Follow these steps to set up the project on your local system:

### Prerequisites

- Node.js and npm should be installed on your system.

### Clone the Repository

```bash
[git clone](https://github.com/your-username/nodejs-authentication.git)
cd nodejs-authentication
```

### Install Dependencies

```bash
npm install
```

### Configure Environment Variables

Create a .env file in the root directory of the project and add the following configuration:

```bash
# Replace these values with your actual configurations
PORT=3000
MONGO_URI=mongodb://localhost:27017/auth_app
SECRET_KEY=your_secret_key
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
RECAPTCHA_SITE_KEY=your_recaptcha_site_key
RECAPTCHA_SECRET_KEY=your_recaptcha_secret_key
```

### Run the Application

```bash
npm start
```

The application should now be running on 
`http://localhost:3000`.

## Folder Structure

The project follows a scalable folder structure to separate models, controllers, and routes. Here's the overview:

```bash
nodejs-authentication/
├── assets/
│   ├── css/
│   │   ├── bootstrap.min.css
│   ├── images/
|   |   ├── backgroundimg.jpg
├── config/
│   ├── checkAuth.js
│   └── keys.js
│   ├── passport.js
├── controllers/
│   ├── authController.js
├── models/
│   ├── User.js
├── node_modules/
│   ├── node modules dependencies
├── routes/
│   ├── authRoutes.js
│   └── indexRoutes.js
├── views/
│   ├── dashboardPage.ejs
│   ├── forgotPasswordPage.ejs
│   ├── layout.ejs
│   ├── loginPage.ejs
│   ├── messages.ejs
│   ├── userRegistrationPage.ejs
│   ├── resetPasswordPage.ejs
│   ├── WelcomePage.ejs
├── .gitignore
├── index.js
├── package-lock.json
├── package.json
```

## Design and Styling

The application's pages are designed to look good and are inspired by authentication systems used by popular services like Google and Facebook. The design uses Bootstrap for responsive layouts and Noty for displaying notifications.

## Password Encryption

User passwords are securely encrypted before being stored in the database. This ensures that sensitive information remains protected even in the event of a data breach.

## Bonus Feature - Forgot Password

The system includes a "Forgot Password" feature that allows users to reset their password. Users can either receive a random password via email or a reset password link, which expires after a certain time (preferred).

## Technologies Used

![MongoDB](/assets/images/mongodb_icon.png)
![ExpressJS](/assets/images/express_icon.png)
![NodeJS](/assets/images/node_icon.png)
![PassportJS](/assets/images/passport_icon.png)
![Bootstrap](/assets/images/bootstrap_icon.png)


## Important Note

Please ensure not to include any passwords or sensitive information in your git commits. Use environment variables and a .env file to manage sensitive data.

# Demo

[NodeJS Authentication](https://auth-web-app-aniket.onrender.com)
