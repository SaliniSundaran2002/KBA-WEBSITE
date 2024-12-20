# KBA WEBSITE  
_A web app to showcase various blockchain-related courses using the MERN stack, with Docker support._

---

## 📖 About
This project is a web application designed to showcase blockchain-related courses. It provides a user-friendly interface for browsing courses, viewing course details, and adding them to a cart. The application is built using the **MERN stack** (MongoDB, Express, React, Node.js) and uses **Docker** for containerization, making the setup and deployment process more efficient.

---

## 🚀 Features
- **Course Listings**: Browse available blockchain courses.
- **Course Details**: View detailed information about each course, including descriptions, prerequisites, and features.
- **Edit and Remove**: Admins can edit or remove courses.

---

## 🛠️ Tech Stack
- **Frontend**: React
- **Backend**: Node.js with Express
- **Database**: MongoDB
- **Containerization**: Docker

---

## 🧑‍💻 Prerequisites

Before you begin, ensure you have the following software installed:

- **Docker**: [Install Docker](https://www.docker.com/get-started)  
- **Node.js**: Version 14 or higher (for local development)
- **npm**: Node Package Manager (usually comes with Node.js)

---

## 📦 Installation with Docker

This project uses **Docker** to containerize the backend and frontend for easier setup and deployment.

### Step 1: Clone the Repository

Clone the repository from GitHub:
    git clone [https://github.com/SaliniSundaran2002/KBA-WEBSITE.git](https://github.com/SaliniSundaran2002/KBA-WEBSITE.git)
    
   cd KBA-WEBSITE
   
### Step 2: Set Up Docker Containers

1. Ensure that **Docker** is installed on your machine.  
   You can follow the installation instructions at: https://www.docker.com/get-started

2. **Navigate to the project directory** where the `docker-compose.yml` file is located:

cd path/to/your/project

3. **Create a `.env` file** in the root directory of the project:

touch .env

4. **Open the `.env` file** in your favorite text editor and add the following content:

echo "secretkey=your_secret_key" >> .env

   - Replace `your_secret_key` with your own secret key for JWT authentication.

### Step 3: Build and Run Containers

Build and start the application using Docker Compose:

docker-compose up --build

This command will:
- Build and start the backend, frontend, and MongoDB containers.
- Run the backend API on `http://localhost:5000`.
- Run the frontend React application on `http://localhost:3000`.

### Step 4: Access the Application

- **Frontend**: Open `http://localhost:3000` in your browser to view the course listings and details.
- **Backend API**: The backend server is running on `http://localhost:5000`. You can use this API for handling course data and authentication.
