# 🌍 Wanderlust

**Wanderlust** is a full-stack vacation rental listing platform where users can discover, view, and manage property listings. The application provides a simple and interactive interface for exploring vacation properties along with essential details such as price, location, country, description, and images.

## ✨ Features

* 🏡 **Browse Listings** – View available vacation rental properties.
* 🔍 **Property Details** – View detailed information about each listing.
* ➕ **Create Listings** – Add new vacation rental properties.
* ✏️ **Edit Listings** – Update existing property information.
* 🗑️ **Delete Listings** – Remove listings when required.
* 🖼️ **Property Images** – Display images associated with each property.
* 📍 **Location Information** – Store and display property location and country.
* 💾 **MongoDB Database** – Persist listing information using MongoDB.
* 📱 **Responsive UI** – User-friendly interface built with EJS and Bootstrap/CSS.

## 🛠️ Tech Stack

### Frontend

* EJS
* HTML5
* CSS3
* Bootstrap

### Backend

* Node.js
* Express.js

### Database

* MongoDB
* Mongoose

### Other Tools

* Method-Override
* MongoDB Mongosh
* Git & GitHub
* VS Code

## 🏗️ Project Structure

```text
Wanderlust/
│
├── controllers/
│
├── models/
│   └── listing.js
│
├── routes/
│
├── views/
│   ├── layouts/
│   ├── listings/
│   │   ├── index.ejs
│   │   ├── show.ejs
│   │   ├── new.ejs
│   │   └── edit.ejs
│   │
│   └── includes/
│
├── public/
│   ├── css/
│   └── js/
│
├── init/
│   └── index.js
│
├── data.js
├── app.js
├── package.json
└── README.md
```

> The exact folder structure may vary depending on the current version of the project.

## 🗄️ Database Schema

The project uses a MongoDB database named **`wanderlust`** with a **`listings`** collection.

Each listing contains information such as:

```text
Listing
├── title
├── description
├── image
│   ├── filename
│   └── url
├── price
├── location
└── country
```

## 🔄 Application Workflow

```text
User
  │
  ▼
EJS Frontend
  │
  ▼
Express.js Server
  │
  ▼
Mongoose
  │
  ▼
MongoDB
  │
  ▼
Listings Data
```

### Listing Management Flow

1. User opens the Wanderlust application.
2. Available listings are retrieved from MongoDB.
3. Express.js processes the request.
4. Mongoose communicates with the MongoDB database.
5. EJS renders the listing information on the webpage.
6. Users can create, edit, view, or delete listings.
7. Changes are stored persistently in MongoDB.

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone <your-github-repository-url>
```

### 2. Navigate to the Project

```bash
cd Wanderlust
```

### 3. Install Dependencies

```bash
npm install
```

### 4. Start MongoDB

Make sure MongoDB is running locally.

The application uses the `wanderlust` database.

### 5. Initialize Sample Data

If the project contains the initialization script:

```bash
node init/index.js
```

This can be used to populate the database with sample listings.

### 6. Start the Server

```bash
node app.js
```

Or, if a start script is configured:

```bash
npm start
```

### 7. Open the Application

Visit:

```text
http://localhost:8080
```

## 📌 CRUD Operations

Wanderlust implements the basic CRUD operations:

| Operation  | Purpose                         |
| ---------- | ------------------------------- |
| **Create** | Add a new property listing      |
| **Read**   | View existing property listings |
| **Update** | Modify listing details          |
| **Delete** | Remove a listing                |

For updating listings, the application uses **Method-Override** to support HTTP `PUT` requests through forms.

Example:

```text
/listings/:id?_method=PUT
```

## 📚 Key Concepts Used

This project helped implement and understand several full-stack development concepts:

* RESTful routing
* CRUD operations
* MVC-style application structure
* Express.js routing
* MongoDB database operations
* Mongoose schemas and models
* EJS templating
* EJS layouts
* Form handling
* Method Override
* Server-side rendering
* Database persistence
* Static files and CSS
* Middleware in Express.js

## 🎯 Learning Outcomes

Through Wanderlust, the following concepts were practiced:

* Building a backend using **Node.js and Express.js**
* Connecting an application to **MongoDB**
* Working with **Mongoose models and schemas**
* Creating RESTful routes
* Implementing complete CRUD functionality
* Rendering dynamic pages using **EJS**
* Structuring a full-stack web application
* Managing data persistence
* Designing a responsive frontend using **Bootstrap/CSS**

## 🔮 Future Enhancements

Possible improvements for the project include:

* 🔐 User authentication and authorization
* ⭐ Ratings and reviews
* 🔎 Advanced search and filtering
* 🗺️ Interactive maps
* ❤️ Wishlist/favorites
* 📅 Booking and reservation system
* 💳 Online payment integration
* ☁️ Cloud image storage
* 📱 Improved mobile responsiveness

## 👩‍💻 Author

**Riya**

B.Tech – Artificial Intelligence & Data Science

---

⭐ If you found this project useful, consider giving the repository a star!
