[![Node.js](https://img.shields.io/badge/Node.js-18.x-green?logo=node.js)](https://nodejs.org/)
[![MongoDB](https://img.shields.io/badge/MongoDB-Atlas%20or%20Local-green?logo=mongodb)](https://mongodb.com/)

A backend application that manages online contests where users can participate, submit answers, and view leaderboards.
Admins can create contests and add questions, while users can join based on their roles.

🚀 Features

✅ Role-based Access Control

Admin: Create contests, add questions, manage leaderboard

VIP User: Can access both VIP & Normal contests

Normal User: Can access only Normal contests

Guest: Can only view contests (cannot participate)

✅ Contest Management

Create contests with name, description, start/end time, and prize

Add different question types (Single-select, Multi-select, True/False)

✅ Participation & Scoring

Users can submit answers and get automatically scored

Correct answers give +1 point

No negative marking

✅ Leaderboard

Displays users sorted by highest score

✅ Authentication

JWT-based login & signup

Protected routes using middleware

✅ Error Handling & Security

Centralized error handling

Rate limiting for auth routes

Helmet & CORS enabled

🛠️ Tech Stack

Backend

🟢 Node.js

🚂 Express.js

🍃 MongoDB (Mongoose ORM)

🔐 JWT for Authentication

🧰 Express Middlewares

Development Tools

🧩 Postman for testing

⚙️ Nodemon for auto reload

📦 dotenv for environment variables

⚙️ Setup Instructions
1️⃣ Clone the Repository
```
git clone https://github.com/your-username/contest-management-system.git
cd contest-management-system/backend
```

2️⃣ Install Dependencies
```
npm install
```

3️⃣ Create .env File

Create a .env file in your backend folder:
```
MONGO_URI=mongodb://127.0.0.1:27017/contestdb
JWT_SECRET=supersecretkey
PORT=5050
```

4️⃣ Run the Server
```
npm run dev
```

✅ Server starts on:

```
http://localhost:5050
```

✅ MongoDB connected successfully:

✅ MongoDB connected successfully

🧪 API Endpoints
🔐 Auth Routes
Method	    Endpoint	    Description
POST	  /auth/register	  Register new user (Admin/VIP/Normal)
POST	/auth/login	        Login and get JWT token

🏁 Contest Routes
Method	  Endpoint	                Description	Access
POST	/contest/	                    Create new contest	Admin
POST	/contest/:contestId/question	Add question to contest	Admin
GET	/contest/	                      Fetch contests (filtered by role)	All Authenticated Users
POST	/contest/submit	              Submit answers for scoring	Normal/VIP Users

🏅 Leaderboard Route
Method	Endpoint	        Description	Access
GET	    /leaderboard/	      Fetch leaderboard sorted by score	All Authenticated Users

🧾 Scoring Rules

✅ Correct answer → +1 point

❌ Incorrect answer → 0 points

No negative marking

Multi-select must match all correct options for +1 point

# MongoDB Atlas

Replace .env MONGO_URI with your connection string:
```
MONGO_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/contestdb
```

🔐 Authentication Header Format

Authorization: Bearer <TOKEN>

Example:

Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...

💬 Example Testing Flow

1️⃣ Register Admin → /auth/register
2️⃣ Login Admin → /auth/login
3️⃣ Create Contest → /contest/
4️⃣ Add Questions → /contest/:id/question
5️⃣ Register Normal User → /auth/register
6️⃣ Login Normal User → /auth/login
7️⃣ Submit Answers → /contest/submit
8️⃣ Check Leaderboard → /leaderboard/

🙋‍♂️ Author

Aryan Sinha
* [![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/aryan-sinha-877698212/)

* [![gmail](https://img.shields.io/badge/gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:aryan.sinha1818@gmail.com)
