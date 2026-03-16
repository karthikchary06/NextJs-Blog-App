# Blog App – Next.js

A simple **Blog Management Application** built with Next.js using the App Router.
This project allows users to create, view, update, and delete blog posts through API routes.

---

## 🚀 Tech Stack

* Next.js (App Router)
* React
* MongoDB
* Mongoose
* Joi (Validation)
* Tailwind CSS
* shadcn/ui components

---

## 📁 Project Structure

```
src
 ├── app
 │   ├── api
 │   │   ├── add-blog
 │   │   │   └── route.js
 │   │   ├── delete-blog
 │   │   │   └── route.js
 │   │   ├── get-blogs
 │   │   │   └── route.js
 │   │   └── update-blog
 │   │       └── route.js
 │   ├── blogs
 │   │   └── page.js
 │   ├── favicon.ico
 │   ├── globals.css
 │   ├── layout.js
 │   └── page.js
 │
 ├── components
 │   ├── add-new-blog
 │   │   └── index.js
 │   ├── blog-overview
 │   │   └── index.js
 │   └── ui
 │       ├── button.jsx
 │       ├── card.jsx
 │       ├── dialog.jsx
 │       ├── input.jsx
 │       └── label.jsx
 │
 ├── database
 │   └── index.js
 │
 ├── lib
 │   └── utils.js
 │
 └── models
     └── blog.js
```

---

## ⚙️ Features

* Add new blog posts
* View all blogs
* Update existing blogs
* Delete blogs
* Form validation using Joi
* MongoDB database integration
* Reusable UI components with shadcn/ui

---

## 🔌 API Routes

| Method | Endpoint           | Description       |
| ------ | ------------------ | ----------------- |
| POST   | `/api/add-blog`    | Create a new blog |
| GET    | `/api/get-blogs`   | Fetch all blogs   |
| PUT    | `/api/update-blog` | Update a blog     |
| DELETE | `/api/delete-blog` | Delete a blog     |

---

## 🗄 Database

MongoDB is used as the database and connected using Mongoose.

Example schema:

```js
import mongoose from "mongoose";

const blogSchema = new mongoose.Schema({
  title: String,
  description: String
});

const Blog = mongoose.models.Blog || mongoose.model("Blog", blogSchema);

export default Blog;
```

---

## ▶️ Running the Project

Install dependencies:

```
npm install
```

Run development server:

```
npm run dev
```

Open in browser:

```
http://localhost:3000
```

---

## 📌 Pages

| Route    | Description          |
| -------- | -------------------- |
| `/`      | Homepage             |
| `/blogs` | Blog management page |

---

## 📦 Components

* **Add New Blog** – Form to create blog posts
* **Blog Overview** – Displays list of blogs
* **UI Components** – Button, Card, Dialog, Input, Label

---

## 🧠 Learning Purpose

This project demonstrates:

* Next.js App Router API routes
* CRUD operations with MongoDB
* Form validation with Joi
* Component-based architecture
* Reusable UI components with shadcn/ui

---

## 👨‍💻 Author

Karthik Chary
