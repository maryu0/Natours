# 🌿 Natours — Nature Tours for Adventurers
*A full-featured travel booking API built using Node.js, Express, MongoDB, and Mongoose.*

Natours is a **complete RESTful API** for a fictional nature-tour company.  
It includes advanced features like authentication, authorization, geospatial queries, image uploading, and more — all built following modern backend best practices.

---

## 🚀 Features

### 🔐 Authentication & Authorization
- User signup & login using **JWT**
- Password hashing with **bcrypt**
- **Role-based access control** (user, guide, lead-guide, admin)
- Protected tours & reviews

### 🌍 Tours API
- Create, update, delete tours  
- Sorting, filtering, pagination  
- Geospatial queries: *"tours within X km"*
- Aggregation pipeline for stats  
- Virtual properties & population

### 👤 Users API
- Update profile & password
- Upload and process profile photos (Sharp)
- Account deactivation
- Secure user roles

### ⭐ Reviews API
- Nested routes: `/tours/:tourId/reviews`
- Users can create/update/delete reviews  
- Tour rating calculations

### 🔒 Security Features
- Rate limiting  
- Data sanitization  
- HTTP security headers with Helmet  
- Preventing parameter pollution  
- Global error handling middleware  

---

## 🛠️ Tech Stack
- **Node.js**
- **Express.js**
- **MongoDB**
- **Mongoose**
- **JWT + Cookies**
- **Multer & Sharp**
- **Nodemailer / Email utils**

---

## 📦 Installation & Setup

### 1️ Clone the repo
```bash
git clone https://github.com/yourusername/Natours.git
cd Natours
```
### 2️ Install dependencies
npm install

### 3 Create a .env file (in project root) and add required environment variables:
NODE_ENV=development
PORT=3000

- MongoDB (example Atlas)
DATABASE=mongodb+srv://<username>:<password>@cluster0.xxxxxx.mongodb.net/natours
DATABASE_PASSWORD=<your-password>

- JWT
JWT_SECRET=your_jwt_secret
JWT_EXPIRES_IN=90d
JWT_COOKIE_EXPIRES_IN=90

- Email (optional)
EMAIL_USERNAME=your_email_username
EMAIL_PASSWORD=your_email_password
EMAIL_HOST=smtp.example.com
EMAIL_PORT=587

### 4 Start the server
```bash
npm run dev
```
