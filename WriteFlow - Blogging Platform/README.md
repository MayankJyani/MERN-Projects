# ✨ WriteFlow — Modern Blogging Platform

Welcome to **WriteFlow** — a vibrant, feature-rich platform for creators to write, publish, and manage blogs with style and ease.

---

<p align="center">
  <img src="https://img.shields.io/badge/Tech-React%20%7C%20Node.js%20%7C%20MongoDB-informational?style=flat-square" />
  <img src="https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square" />
</p>

---

## 🚀 Features

- **📝 Rich Post Editor:**  
  Compose beautiful posts with titles, content, images, categories, and tags.

- **💾 Drafts, Publishing, & Scheduling:**  
  Save drafts, publish instantly, or schedule posts for the future.

- **🌄 Image Uploads:**  
  Add a featured image to your post for extra flair.

- **⚡ Real-Time Activity:**  
  Get instant updates when new posts are published or scheduled.

- **👤 Personal Dashboard:**  
  View, edit, and manage all your posts, organized by status.

- **🏷️ Categories & Tags:**  
  Effortlessly organize and discover content.

- **🔒 Secure Authentication:**  
  Protect your work with JWT-based user authentication.

- **🛠️ RESTful API:**  
  Full CRUD support for blog management.

---

## 🌟 Why WriteFlow?

> “Experience blogging like never before with our innovative platform designed for creators.”

WriteFlow brings together beauty, simplicity, and power for an unforgettable writing journey.

---

## 🛠️ Getting Started

### Prerequisites

- **Node.js** (v18+)
- **MongoDB** (local or remote)
- **Cloudinary** (for image hosting)
- **npm** or **yarn**

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/MayankJyani/Blogging_platform.git
cd Blogging_platform

# 2. Install server dependencies
cd server
npm install

# 3. Install client dependencies
cd ../client
npm install
```

### Environment Setup

Create a `.env` file in `server/`:

```
MONGODB_URI=your_mongodb_connection_string
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
JWT_SECRET=your_jwt_secret
```

---

### Running the Platform

```bash
# Start the backend (from server/)
npm start

# Start the frontend (from client/)
npm run dev
```

---

## 🖥️ Usage

1. **Sign Up / Log In** to access your dashboard.
2. **Create Posts** — Add title, content, images, tags, and more.
3. **Save as Draft, Publish, or Schedule** your posts.
4. **Manage Your Content** from your personal dashboard.
5. **Enjoy Real-Time Updates** as new content is created across the platform!

---

## ⚙️ Tech Stack

- **Frontend:** React, Vite, Lucide Icons, modern UI libraries
- **Backend:** Node.js, Express.js, MongoDB, Mongoose
- **Cloud Storage:** Cloudinary
- **Auth:** JWT

---

## 📂 Project Structure

```
Blogging_platform/
┣ 📂 backend
┃ ┣ 📂 controllers # Route logic (auth, posts, comments, likes, admin)
┃ ┣ 📂 models # MongoDB models (User, Blog, Comment, Like)
┃ ┣ 📂 routes # API routes (auth, posts, users, admin)
┃ ┣ 📂 middleware # Auth & validation middleware
┃ ┣ server.js # Main backend entry
┣ 📂 frontend
┃ ┣ 📂 src
┃ ┃ ┣ 📂 components # Reusable UI components
┃ ┃ ┣ 📂 pages # Main app pages (Login, Dashboard, Profile, etc.)
┃ ┃ ┣ 📂 hooks # Custom React hooks
┃ ┃ ┣ 📂 utils # Helpers & API config
┃ ┃ ┗ App.jsx # Main app entry
┣ 📄 package.json
┣ 📄 README.md

```

---

## 📝 License

MIT © [MayankJyani](https://github.com/MayankJyani)

---

## 👏 Acknowledgements

> Inspired by the passion of creators who want a beautiful, intuitive space to share their ideas.

---

## Some SneakPeak -

<img width="1912" height="937" alt="image" src="https://github.com/user-attachments/assets/b7969842-bac6-459a-95d6-58a928e61965" />
<img width="1897" height="930" alt="image" src="https://github.com/user-attachments/assets/ab519ad7-6957-4a22-a448-28ad5f555bac" />
<img width="1907" height="927" alt="image" src="https://github.com/user-attachments/assets/a77926d0-cd5f-4b88-bbde-b3c99d60f963" />
<img width="1910" height="842" alt="image" src="https://github.com/user-attachments/assets/97dc4925-8425-4fc6-b736-ab5483b5e2aa" />
<img width="1918" height="937" alt="image" src="https://github.com/user-attachments/assets/ea309332-ccfe-419a-a629-6c661862bf2c" />
<img width="1913" height="917" alt="image" src="https://github.com/user-attachments/assets/53035c1b-3727-42da-9021-9a2ab2dabfca" />
<img width="1918" height="933" alt="image" src="https://github.com/user-attachments/assets/c3c28591-1758-4e6f-b894-eaf361bc7e65" />
<img width="1918" height="933" alt="image" src="https://github.com/user-attachments/assets/daed9415-87d9-42ef-9707-39fa5d005144" />
<img width="1918" height="936" alt="image" src="https://github.com/user-attachments/assets/7a5b2e7d-343c-4458-89c9-98491211459e" />
<img width="1918" height="932" alt="image" src="https://github.com/user-attachments/assets/1e7d677d-63b2-48b0-b8aa-32333bc6de21" />
<img width="1918" height="937" alt="image" src="https://github.com/user-attachments/assets/eb7b4ea6-f64c-4b0c-af10-8e1ab2366990" />





<p align="center">
  <b>Ready to write? Start your journey with WriteFlow! 🚀</b>
</p>
