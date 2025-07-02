# CINEMATRIX
# 🎬 CineMatrix - Movie Booking System

CineMatrix is a full-stack movie ticket booking application where users can browse movies, view showtimes, select seats, and book tickets. Admins can manage theaters, screens, shows, and movies.

---

## 📌 Features

### ✅ User Features
- 🎞 Browse movies by city, genre, or language
- 🏛 View theater-wise showtimes
- 🎟 Book movie tickets with seat selection (Silver, Gold, Platinum)
- 📖 View personal bookings
- 👤 User profile management

### ✅ Admin Features
- ➕ Add and manage theaters (name, location, city, pincode)
- ➕ Add screens with seat capacity
- 🕒 Add shows by selecting movie, screen, time
- 🎥 Add movies manually or via OMDB API
- 🎫 Auto-generate seats dynamically based on screen capacity

---

## 💻 Tech Stack

### Frontend (React + Tailwind CSS)
- React Router
- Axios
- React Toastify
- Framer Motion (animations)
- Role-based routes (User/Admin)

### Backend (Spring Boot)
- Spring Boot 3
- Spring Security + JWT Authentication
- Hibernate + JPA
- MySQL (relational DB)
- OMDB API integration (for movie metadata)

---

## 🧱 Project Structure

### Backend

src/
├── controller/
├── dto/
├── model/
├── repository/
├── service/
├── exception/
└── config/



### Frontend

src/
├── api/
├── components/
│ └── common/
├── context/
├── pages/
│ ├── admin/
│ └── user/
├── utils/
└── App.js, index.js

yaml


---

## 🚀 Getting Started
### ✅ Prerequisites

- Node.js (v18+)
- Java 17+
- MySQL 8+
- Maven
## 🛠 Setup
### ⚙ Backend

1. Clone the repo
2. Configure application.properties:
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/cinematrix
   spring.datasource.username=root
   spring.datasource.password=your_password
Run the backend:
mvn spring-boot:run
🌐 Frontend
Navigate to /frontend folder
Install dependencies:
npm install
Start dev server:
npm start
🔐 Admin Registration (Secure)
To prevent users from registering as admins:
Admin registration is done only via /admin-register?key=SECRET_KEY
Admins can then log in via /login
🪑 Seat Generation Logic
When an admin adds a show, seats are auto-generated
Seat layout is dynamic based on screen capacity
Types are divided as:
First 40% ➤ SILVER
Next 30% ➤ GOLD
Last 30% ➤ PLATINUM
📸 Screenshots
<Add screenshots of Home, Booking, Admin Dashboard, etc. here>
Full-stack Developer | Java + React | Spring Boot | MySQL
