# QurbaniHat – Livestock Booking Platform

## Project Overview

QurbaniHat is a modern livestock booking platform built for Qurbani animal browsing and reservation. Users can explore verified cows and goats, view detailed animal information, compare animals by price, weight, breed, and location, and place booking requests after authentication. The project includes email/password authentication, optional Google login, protected private routes, profile management, and a responsive user interface.

## Live Project Link

Live Website: https://qurbani-hat-assignment-08-4wk6.vercel.app



## Technologies Used

- Next.js
- React.js
- Tailwind CSS
- Better Auth
- MongoDB
- Better Auth MongoDB Adapter
- React Icons
- React Toastify
- Lottie React
- Vercel Deployment

## Core Features

- Modern livestock marketplace homepage.
- Users can browse available Qurbani animals.
- Users can view cows and goats with image, price, breed, weight, age, location, and category.
- Featured animals section on the homepage.
- All animals page with verified animal listing.
- Sort animals by price from low to high or high to low.
- Animal details page with full animal information.
- Protected booking page behavior for authenticated users.
- Users must log in before placing a booking request.
- Booking form with name, email, phone, and address fields.
- Email and password authentication using Better Auth.
- Optional Google login support.
- MongoDB database integration for authentication data.
- Protected private route for user profile.
- User profile page.
- Update profile information using Better Auth.
- Responsive navbar with login, register, profile, and logout options.
- Toast notifications for user actions.
- Custom not-found and loading pages.
- Fully responsive design for mobile, tablet, and desktop.

## Dependencies Used

### Main Dependencies

```json
{
  "@better-auth/mongo-adapter": "^1.6.9",
  "better-auth": "^1.6.9",
  "lottie-react": "^2.4.1",
  "mongodb": "^6.20.0",
  "next": "16.2.4",
  "react": "19.2.4",
  "react-dom": "19.2.4",
  "react-icons": "^5.6.0",
  "react-toastify": "^11.0.5"
}
```

### Development Dependencies

```json
{
  "@tailwindcss/postcss": "^4.1.18",
  "tailwindcss": "^4.1.18",
  "eslint": "^9.39.1",
  "eslint-config-next": "16.2.4"
}
```

## How to Run the Project Locally

### 1. Clone the Repository

```bash
git clone your-repository-link
cd QurbaniHat-main
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Create Environment File

Create a `.env.local` file in the project root and add the following environment variables:

```env
BETTER_AUTH_SECRET=your-better-auth-secret
BETTER_AUTH_URL=http://localhost:3000
NEXT_PUBLIC_APP_URL=http://localhost:3000

MONGODB_URI=your-mongodb-atlas-uri
MONGODB_DATABASE=qurbanihat

NEXT_PUBLIC_ENABLE_GOOGLE_AUTH=false
GOOGLE_CLIENT_ID=
GOOGLE_CLIENT_SECRET=
```

If you want to use Google login, set:

```env
NEXT_PUBLIC_ENABLE_GOOGLE_AUTH=true
GOOGLE_CLIENT_ID=your-google-client-id
GOOGLE_CLIENT_SECRET=your-google-client-secret
```

### 4. Generate Better Auth Secret

You can generate a secure Better Auth secret using:

```bash
npm run secret
```

Copy the generated value and paste it into:

```env
BETTER_AUTH_SECRET=your-generated-secret
```

### 5. Test MongoDB Connection

```bash
npm run test-db
```

### 6. Run the Development Server

```bash
npm run dev
```

### 7. Open the Project in Browser

```text
http://localhost:3000
```

## Available Scripts

```bash
npm run dev
```

Runs the project in development mode.

```bash
npm run build
```

Builds the project for production.

```bash
npm run start
```

Starts the production server.

```bash
npm run lint
```

Runs ESLint checking.

```bash
npm run secret
```

Generates a Better Auth secret.

```bash
npm run test-db
```

Tests the MongoDB Atlas connection.

## Environment Variables

| Variable Name | Description |
|---|---|
| `BETTER_AUTH_SECRET` | Secret key for Better Auth |
| `BETTER_AUTH_URL` | Base URL for Better Auth |
| `NEXT_PUBLIC_APP_URL` | Public app URL |
| `MONGODB_URI` | MongoDB Atlas connection string |
| `MONGODB_DATABASE` | MongoDB database name |
| `NEXT_PUBLIC_ENABLE_GOOGLE_AUTH` | Enables or disables Google login |
| `GOOGLE_CLIENT_ID` | Google OAuth client ID |
| `GOOGLE_CLIENT_SECRET` | Google OAuth client secret |

## Relevant Resources

Live Website: https://qurbani-hat-assignment-08-4wk6.vercel.app

