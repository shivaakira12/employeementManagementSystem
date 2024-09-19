

---

# 🌟 Employee Management System (EMS) 🌟

## 📝 Project Overview
The **Employee Management System (EMS)** is a full-stack web application where:
- 🧑‍💼 **Employees** can apply for leave, check salary options, and view their leave statuses.
- 👩‍💻 **Admins** can manage employees, add departments, approve leave requests, and manage employee salaries.

## 🚀 Features
- **Employee Features:**
  - 📅 Apply for leave.
  - 👁 View applied leaves.
  - 💰 Check salary details.
  
- **Admin Features:**
  - ➕ Add new employees.
  - 🏢 Manage departments.
  - ✅ Approve/Reject leave requests.
  - 💼 Manage employee salaries.

## 🛠 Technologies Used

### 🖥️ Frontend:
- **Framework**: [React](https://reactjs.org/) (Vite setup)
- **Styling**: [Tailwind CSS](https://tailwindcss.com/), [Styled Components](https://styled-components.com/)
- **Routing**: [React Router DOM](https://reactrouter.com/en/main)
- **Icons**: [React Icons](https://react-icons.github.io/react-icons/)
- **HTTP Client**: [Axios](https://axios-http.com/)
- **Tables**: [React Data Table Component](https://www.npmjs.com/package/react-data-table-component)

### ⚙️ Backend:
- **Framework**: [Express.js](https://expressjs.com/)
- **Database**: [MongoDB](https://www.mongodb.com/) (via Mongoose)
- **Authentication**: [JWT](https://jwt.io/) (JSON Web Tokens)
- **Password Encryption**: [Bcrypt](https://www.npmjs.com/package/bcrypt)
- **File Uploads**: [Multer](https://www.npmjs.com/package/multer)
- **CORS**: [cors](https://www.npmjs.com/package/cors) (Cross-Origin Resource Sharing)

---

## ⚙️ Installation Instructions

### Prerequisites:
- 🔧 **Node.js** and **npm** installed.
- 🗄 **MongoDB** installed locally or a MongoDB cloud instance.
  
### Cloning the repository:
```bash
git clone https://github.com/shivaakira12/employeementManagementSystem.git
```

### 🚧 Frontend Setup (Vite):
1. Navigate to the frontend folder:
   ```bash
   cd employeementManagementSystem/frontend
   ```

2. Install frontend dependencies:
   ```bash
   npm install
   ```

3. Start the frontend development server:
   ```bash
   npm run dev
   ```

### 🛠 Backend Setup (Express):
1. Navigate to the server folder:
   ```bash
   cd ../server
   ```

2. Install backend dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file in the `server` directory and add the following environment variables:
   ```bash
   PORT=3000
   MONGO_URI=your_mongo_database_connection_string
   JWT_SECRET=your_secret_key
   ```

4. Start the backend server:
   ```bash
   npm start
   ```

---

## 🗂 Project Structure

### Frontend (`/frontend`)
```plaintext
├── components     // 🛠 React components like Header, Sidebar, etc.
├── pages          // 📄 Main pages like Employee Dashboard, Admin Dashboard, etc.
├── utils          // 🔧 Utility functions and constants
└── App.jsx        // 🏗️ Main app file
```

### Backend (`/server`)
```plaintext
├── index.js       // 🏁 Main server file
├── models         // 🗄️ MongoDB models for Employee, Department, Leave, etc.
├── routes         // 🌐 Express routes for employee and admin functionality
└── middleware     // 🔒 Middleware for authentication (JWT, etc.)
```

---

## 🛠 Available Scripts

### Frontend:
- `npm run dev`: Runs the app in development mode. Open [http://localhost:3000](http://localhost:3000) to view it in the browser.
  
### Backend:
- `npm start`: Runs the backend server using nodemon for hot-reloading.

---

## 🔌 API Endpoints

### 🧑‍💼 Admin:
- `POST /api/admin/add-employee`: ➕ Adds a new employee to the system.
- `POST /api/admin/add-department`: 🏢 Adds a new department.
- `GET /api/admin/leaves`: 👁 Retrieves all pending leave requests for approval.
- `PATCH /api/admin/leave/:id/approve`: ✅ Approves a leave request.

### 👨‍💻 Employee:
- `POST /api/employee/apply-leave`: 📅 Apply for a new leave.
- `GET /api/employee/leaves`: 👁 View applied leave status.
- `GET /api/employee/salary`: 💰 Check salary details.

---

## 🎨 Tailwind CSS Configuration
Tailwind CSS has been configured in the `frontend` application. To modify or add custom styles:
1. Open the `tailwind.config.js` file.
2. Adjust settings as needed for your project’s styling.

```javascript
module.exports = {
  content: ['./index.html', './src/**/*.{js,ts,jsx,tsx}'],
  theme: {
    extend: {},
  },
  plugins: [],
};
```

---

## 📈 Future Enhancements
- Implementing 🔐 **role-based authentication** for admin and employee.
- Detailed 💼 **salary management** for employees.
- Departmental 🏢 **performance tracking**.

---

