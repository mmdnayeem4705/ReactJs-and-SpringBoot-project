# 🎯 Hobby Management Full Stack Application

A full-featured full-stack web application built using **ReactJS** for the frontend and **Spring Boot** for the backend. This application allows users to register, create and manage hobby listings, update profiles, and interact with a secure user system including roles like admin, business owners, and general users.

---

## 📌 Features

### 🔐 Authentication & Authorization
- Sign Up / Login functionality
- User roles: `USER`, `ADMIN`, and `BUSINESS_USER`
- Password encryption with BCrypt
- JWT-based session management

### 🎭 User Types
- **AppClient** (general users): Can view and register for hobbies
- **BusinessOwner**: Can create, manage and delete hobbies

### 📦 Hobby Management
- Add / Edit / Delete hobbies (for businesses)
- Save / Match hobbies (for users)
- View hobby recommendations

### 🌐 Technologies Used

#### 🧩 Frontend (ReactJS)
- ReactJS with Hooks
- React Router
- Axios for API integration
- Tailwind CSS for UI styling
- Toast Notifications

#### 🚀 Backend (Spring Boot)
- Spring Web MVC
- Spring Security + JWT
- Hibernate / JPA for DB operations
- MySQL for database
- Swagger UI for API documentation
- Cloudinary API integration for image upload
- Email service via Gmail SMTP

---

## 📁 Folder Structure

```

📦 ReactJS-Spring-Boot-Full-Stack-App-main
├── backend.hobbiebackend          # Spring Boot backend
│   ├── controller
│   ├── model (entities, enums, DTOs)
│   ├── repository
│   ├── service
│   └── configuration
├── react-frontend                 # ReactJS frontend
│   ├── public
│   └── src
│       ├── components
│       ├── pages
│       └── App.jsx

```

---

## ⚙️ Getting Started

### ✅ Prerequisites
- Java 11 or above
- Node.js & npm
- MySQL Server
- Maven
- Git

### 🔧 Backend Setup

1. Clone the repo and open `backend.hobbiebackend` in IDE (e.g., IntelliJ)
2. Create MySQL DB:
```

CREATE DATABASE hobbie\_backend\_db;

````
3. Update `application.properties`:
```properties
spring.datasource.username=root
spring.datasource.password=your_password
cloudinary.cloud-name=your_cloud_name
cloudinary.api-key=your_api_key
cloudinary.api-secret=your_api_secret
````

4. Run the Spring Boot App:

   ```
   mvn spring-boot:run
   ```

---

### 🎨 Frontend Setup

1. Navigate to frontend directory:

   ```
   cd react-frontend
   ```
2. Install dependencies:

   ```
   npm install
   ```
3. Start development server:

   ```
   npm start
   ```

---

## 🧪 API Documentation

Visit Swagger UI once backend is running:

```
http://localhost:8080/swagger-ui.html
```

---

## 🗃️ Database Schema

* `users`
* `roles`
* `users_roles` (many-to-many)
* `hobbies`
* `posts`
* `app_client`, `business_owner` (joined inheritance)

---

## 🔐 Security

* BCrypt password encryption
* JWT Token-based authentication
* Role-based authorization

---

## 📸 Image Uploading

* Cloudinary is used to store uploaded hobby images.
* Requires a Cloudinary account.

---

## 📧 Email Integration

* App sends confirmation emails via Gmail SMTP
* Setup credentials in `application.properties`:

  ```properties
  spring.mail.username=your_email@gmail.com
  spring.mail.password=your_app_password
  ```

---

## 🧑‍💻 Author

**M Mohammed Nayeem**
GitHub: [@mmdnayeem4705](https://github.com/mmdnayeem4705)
LinkedIn: [@Mulla Mohammed Nayeem](https://www.linkedin.com/in/mulla-mohammed-nayeem-09b33a361/)

---

## 📜 License

This project is licensed under the MIT License.

```

---

Would you like me to create this `README.md` file inside your project directory automatically or generate a downloadable copy?
```

