[![Node.js](https://img.shields.io/badge/Node.js-18.x-green?logo=node.js)](https://nodejs.org/)
[![Express.js](https://img.shields.io/badge/Express.js-Backend-black?logo=express)](https://expressjs.com/)
[![MongoDB](https://img.shields.io/badge/MongoDB-Atlas%20or%20Local-green?logo=mongodb)](https://mongodb.com/)
[![Mongoose](https://img.shields.io/badge/Mongoose-ODM-red?logo=mongoose)](https://mongoosejs.com/)
[![JWT](https://img.shields.io/badge/JWT-Authentication-orange?logo=jsonwebtokens)](https://jwt.io/)
[![Postman](https://img.shields.io/badge/Postman-API%20Testing-orange?logo=postman)](https://www.postman.com/)
[![Git](https://img.shields.io/badge/Git-Version%20Control-black?logo=git)](https://git-scm.com/)

# 🏆 Contest App Backend
The Contest App is a robust and scalable server built using Node.js, Express.js, and MongoDB.
It handles all the core logic for managing contests, users, and questions including secure authentication, contest creation, question tracking, and real-time score evaluation. Designed with modular architecture and clean APIs.


### 🚀 Features

✅ User Registration & Login (JWT-based authentication)
🏁 Create, Fetch, and Manage Contests
📚 Add, Retrieve, and Evaluate Contest Questions
💾 MongoDB (Atlas or Local) Database Support
🔐 Secure Endpoints using Middleware Authentication
🌍 Environment-based Configurations (via .env)

🛠️ Tech Stack
Component	    Technology
Runtime	        Node.js
Framework	      Express.js
Database	      MongoDB / Mongoose
Authentication	JSON Web Token (JWT)
Environment	    dotenv

⚙️ Project Setup
1️⃣ Clone the repository
```
git clone https://github.com/aryansinha1818/contest-backend.git
cd contest-backend
```

2️⃣ Install dependencies
```
npm install
```

3️⃣ Configure environment variables

Create a .env file in the root directory and add:

```
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
```

4️⃣ Start the server

For development:
```
npm run dev
```

For production:
```
npm start
```

🧪 Testing the APIs

You can use:

* Postman
* Thunder Client (VS Code extension)
* or cURL

Example:
```
GET http://localhost:5000/api/contests
```

🙋‍♂️ Author

Aryan Sinha
* [![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/aryan-sinha-877698212/)

* [![gmail](https://img.shields.io/badge/gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:aryan.sinha1818@gmail.com)
