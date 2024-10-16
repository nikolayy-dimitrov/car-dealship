# NamCar Dealership Demo
[Live preview](https://namcar.site/)

## Overview
NamCar Dealership is a web application project offering its users the ability to browse, 
sell and purchase vehicles. With a functional sign up and login system. It is built with TypeScript, React, Vite, Tailwind CSS, MySQL, Node.js, Express. 
It is entirely hosted on the AWS platform, utilizing Nginx and PM2 for routing and uptime.

## Features

- **User Authentication:** Secure login and registration for users.
- **Car Listings Management:** Add, update, and delete cars from the dealership inventory.
- **Search & Filters:** Advanced search options for users to find cars based on make, model, year, and more.
- **Responsive Design:** Works seamlessly across mobile, tablet, and desktop devices.
- **Cloud Storage:** Store images and media assets in AWS S3.
- **Availability:** Deployed with uptime monitoring and load balancing on AWS.

## Tech Stack

### Frontend
- **Vite:** Lightning-fast development environment with an optimized build process.
- **React.js:** Component-based architecture for building dynamic user interfaces.
- **Tailwind CSS:** Utility-first CSS framework for building custom designs without leaving your HTML.
- **TypeScript:** Typed JavaScript for improved development experience and code quality.

### Backend
- **Node.js & Express.js:** RESTful API for server-side logic and routing.
- **MySQL:** Relational database for storing car listings, user data, and transactions.
- **TypeScript:** Ensuring type safety and better tooling in the backend.
- **JWT Authentication:** JSON Web Token for secure authentication.
- **AWS EC2:** The application is hosted on an EC2 instance.
- **AWS S3:** Content, such as car images, is stored in an S3 bucket.
- **Nginx & PM2:** Nginx is used as a reverse proxy, and PM2 manages app uptime and load balancing.

## Screenshots
### Home Page
<img width="1470" alt="Screenshot 2024-10-16 at 11 58 38 AM" src="https://github.com/user-attachments/assets/8aaeb40a-247c-496d-a572-f966f8f174cb">

### Browse listings
<img width="1470" alt="Screenshot 2024-10-16 at 11 59 18 AM" src="https://github.com/user-attachments/assets/a4ab96ef-a300-4b07-a22a-4a7ec647f723">

### List a vehicle
<img width="1470" alt="Screenshot 2024-10-16 at 11 59 50 AM" src="https://github.com/user-attachments/assets/d025f46e-2404-4e71-9203-dbe3056fdd08">

### Sign Up
<img width="1470" alt="Screenshot 2024-10-16 at 11 58 55 AM" src="https://github.com/user-attachments/assets/646873a1-6e15-40c4-b93a-055ba33dd9d8">

### Login
<img width="1470" alt="Screenshot 2024-10-16 at 11 58 50 AM" src="https://github.com/user-attachments/assets/226bf0fb-407a-4c97-ac5a-08904abb8894">

## Installation
### Prerequisites
Ensure you have the following installed:
- **Node.js** (v14 or higher)
- **MySQL** (local or hosted on AWS RDS)

### Steps

1. **Clone the repository:**

   ```bash
   git clone https://github.com/nikolayy-dimitrov/car-dealship.git
   cd car-dealship
   ```
2. **Install dependencies for both frontend and backend:**
   
#### Install backend dependencies
```bash
cd server
npm install
```
#### Install frontend dependencies
```bash
cd ../client
npm install
```

3. **Set up environment variables:**

Create a .env file in the server directory with the following:
```bash
MYSQL_HOST=your_mysql_host
MYSQL_USER=your_mysql_user
MYSQL_PASSWORD=your_mysql_password
MYSQL_DB=your_database_name
JWT_SECRET=your_jwt_secret
AWS_ACCESS_KEY_ID=your_aws_access_key_id
AWS_SECRET_ACCESS_KEY=your_aws_secret_access_key
AWS_S3_BUCKET_NAME=your_s3_bucket_name
PORT=5000
```
4. **Run the application**

# Run the backend server
```bash
cd server
npm start
```
# Run the frontend
```bash
cd ../client
npm run dev
```

## Usage

- Browse the dealership inventory - Users can browse the cars available for sale, search by specific criteria, and view detailed car information.
- Manage car listings - Admin users can log in to add, update, or remove cars from the inventory.
- Authentication - Secure login for both regular users and admin to access additional features.
