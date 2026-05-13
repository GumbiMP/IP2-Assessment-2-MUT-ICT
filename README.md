

MUT ICT Resource Hub is a web-based platform designed to help students access academic resources, notes, and ICT-related information easily. The system allows students and guests to log in, browse resources, and download study materials.

---

Features

* Student Login System
* Guest Registration
* Resource Management
* Notes and File Access
* Search Functionality
* Responsive Design
* Curriculum and Rules Section
* Downloadable Study Materials

---

Technologies Used

| Technology         | Purpose                 |
| ------------------ | ----------------------- |
| HTML               | Frontend Structure      |
| CSS                | Styling                 |
| JavaScript         | Frontend Logic          |
| Node.js            | Backend Runtime         |
| Express.js         | Server Framework        |
| MySQL              | Database                |
| Visual Studio Code | Development Environment |

---

 Project Structure


PROJECT FOLDER
│
├── backend/
│   ├── server.js
│   ├── package.json
│
├── css/
│   ├── styles.css
│
├── js/
│   ├── script.js
│
├── notes/
│
├── index.html
├── login.html
└── README.md
```

---

 Installation Guide

Step 1: Download the Project

Extract the ZIP file into a folder.

---

Step 2: Open Project in VS Code

Open Visual Studio Code and select the project folder.

---

Step 3: Install Node Modules

Open terminal inside the `backend` folder:

cmd
cd backend
npm install


---

# Database Setup

Step 1: Start XAMPP

Start:

* Apache
* MySQL

---

Step 2: Create Database

Open phpMyAdmin and create:

```sql
mut_ict_db
```

---

## Step 3: Import SQL File

Import the provided SQL database file into phpMyAdmin.

---

# Running the Project

Inside the backend folder run:

```bash
node server.js
```

or

```bash
npm start
```

---

# Open the Website

Visit:

```bash
http://localhost:5000
```

---

# API Endpoints

| Endpoint            | Method | Description        |
| ------------------- | ------ | ------------------ |
| /api/login/student  | POST   | Student Login      |
| /api/register/guest | POST   | Guest Registration |
| /api/notes          | GET    | Fetch Notes        |

---

# Frontend and Backend Connection

The frontend communicates with the backend using Fetch API requests.

Example:

```javascript
fetch('/api/login/student', {
    method: 'POST',
    headers: {
        'Content-Type': 'application/json'
    },
    body: JSON.stringify({
        studentNumber,
        password
    })
})
```

The backend processes the request and interacts with the MySQL database.

---

# Database Connection

```javascript
const db = mysql.createConnection({
    host: 'localhost',
    port: 3307,
    user: 'root',
    password: '',
    database: 'mut_ict_db'
});
```

---

# Author

Developed using Visual Studio Code for academic purposes.

---

# License

This project is for educational purposes only.
