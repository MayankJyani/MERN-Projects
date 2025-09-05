# 📊 Excel Analytic Platform

The **Excel Analytic Platform** is a full-stack MERN (MongoDB, Express.js, React, Node.js) application that empowers users to upload, explore, and visualize Excel datasets using AI-powered insights, dynamic charts, and a modern, real-time dashboard interface.

## 🔥 Key Features

### ✅ Excel Upload & Parsing
- Upload `.xls`, `.xlsx` files securely
- Data is parsed and stored in MongoDB using `xlsx`

### 📈 Charting System
- Create interactive **Bar**, **Line**, **Pie**, **Area**, **Radar**, **Scatter**, and **Composed** charts
- Customize X-axis and Y-axis from extracted Excel headers
- View, download (PNG/PDF), and delete charts
- Charts show the **file name**, not just the file ID

### 🧠 AI-Powered Insights
- Automatically generate natural-language insights for uploaded files and charts using **Gemini API**
- Works with fallbacks if AI fails

### 🎯 Chart Recommendations
- Instantly suggest the best chart types based on Excel column patterns
- Shown in a beautiful modal after uploading a file

### 🧭 User Dashboard
- Drag-and-drop or click-to-upload Excel files
- Track:
  - 📁 Total Files Uploaded
  - 📊 Charts Created
  - 💾 Storage Used (MB)
- Beautiful **glare-hover cards** for stats
- Real-time **activity log** for file uploads and chart creations
- Theme-aware responsive UI (light/dark)

### 🚀 Real-Time Notifications
- WebSocket-powered (via **Socket.IO**)
- Live alerts for:
  - File uploads
  - Chart creations
- Grouped by Today / Yesterday / Earlier
- Clickable + “Mark all as read” feature
- Optional toast notifications

### 👤 Authentication & Role Control
- Secure login/register with JWT
- Role-based access: User / Admin
- Passwords hashed with bcrypt
- Profile section with image upload, DOB, and change password

### 🛠 Admin Dashboard
- View platform-wide metrics: Total Users, Uploads, Charts
- List of recent uploads and signups

## 🧩 Tech Stack

| Layer     | Tools |
|-----------|-------|
| Frontend  | React, Vite, Tailwind CSS, Recharts, Framer Motion, React Router, Axios |
| Backend   | Node.js, Express.js, Multer, xlsx, Socket.IO |
| Database  | MongoDB, Mongoose |
| Auth      | JWT, bcrypt |
| AI Engine | Gemini API (Google) |
| Styling   | Tailwind, Lucide Icons |
| Real-Time | Socket.IO, Toast Alerts |

## 🗂 Project Structure

```bash
excel-analytic-platform/
├── server/
│   ├── controllers/       # File, Chart, Auth, AI insight, Recommendation, Admin
│   ├── routes/            # API routing
│   ├── models/            # User, Chart, File schemas
│   ├── middleware/        # JWT auth
│   └── index.js           # Express server & Socket.IO setup
├── src/
│   ├── components/        # UI components (Navbar, Sidebar, Modals, Upload)
│   ├── pages/             # Dashboard (Overview, Files, Charts, Insights)
│   ├── App.jsx            # Main router with nested routes
│   ├── ThemeContext.jsx   # Dark/light toggle
│   └── index.css          # Global styles
```

## ⚙️ Setup Guide

### 1. Clone the Repo
```bash
git clone https://github.com/MayankJyani/Excel-Analytic-Platform.git
cd Excel-Analytic-Platform
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Setup Environment Variables

Create `.env`:
```env
PORT=5000
MONGODB_URI=your_mongodb_uri
JWT_SECRET=your_jwt_secret
GEMINI_API_KEY=your_gemini_api_key
```

### 4. Run the Application

#### Start Backend:
```bash
npm run server
```

#### Start Frontend:
```bash
npm run dev
```

### 5. Access the Platform
Open: [https://exellarts.netlify.app/](https://exellarts.netlify.app/)

---

## 🔗 API Overview

### Auth (`/api/users`)
- `POST /register`, `POST /login`
- `GET /me`, `PUT /me`
- `PUT /password`, `POST /upload-image`

### Files (`/api/files`)
- `POST /upload`
- `GET /secure-route`
- `GET /:id`, `DELETE /:id`
- `GET /headers/:id`
- `GET /stats`

### Charts (`/api/charts`)
- `POST /`, `GET /`, `GET /:id`, `DELETE /:id`

### Admin (`/api/admin`)
- `GET /stats`, `/uploads`, `/users`

### Insights (`/api/insights`)
- `POST /:id/insight`

### Recommendations (`/api/recommend`)
- `GET /recommendations/:fileId`

### Activity Log (`/api/activity`)
- `GET /log`

---

## 🎨 Design Highlights

- 🧭 Elegant dashboards with **animated hover effects**
- 🧠 AI summaries feel natural and smart
- 📦 Glare effect on hover cards (`glare-hover` CSS)
- 📌 Supports deep linking to `/charts?fileId=...&type=...`

---

## Some SneakPeak -
<img width="1918" height="952" alt="image" src="https://github.com/user-attachments/assets/1d5583f7-0263-407b-99cb-70b8c170d504" />
<img width="1918" height="932" alt="image" src="https://github.com/user-attachments/assets/bdbc45a8-17f6-44dd-b519-4acb471e070d" />
<img width="1918" height="936" alt="image" src="https://github.com/user-attachments/assets/9192d783-fe55-46bf-9c26-411a1c10136f" />
<img width="1918" height="937" alt="image" src="https://github.com/user-attachments/assets/202a2cc0-378a-48af-a130-f7d69f28f623" />
<img width="787" height="811" alt="image" src="https://github.com/user-attachments/assets/f3a06a1f-726a-4101-8d13-3476411eb21d" />
<img width="1918" height="927" alt="image" src="https://github.com/user-attachments/assets/c1e686bc-ee58-4e40-b60a-fc5ad871ca3d" />
<img width="1896" height="910" alt="image" src="https://github.com/user-attachments/assets/93f1b3f1-6eb9-41c7-8f33-8376defd306f" />
<img width="1610" height="737" alt="image" src="https://github.com/user-attachments/assets/e9a1bb55-bb9d-45a4-8e53-9be07d4dbd5a" />








## 📄 License

MIT © [Mayank Jyani](https://github.com/MayankJyani)
