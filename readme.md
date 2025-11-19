![TaskHub Logo](https://raw.githubusercontent.com/Tanisboxed/GitPractice/main/taskhubimg.png)

## **TaskHub**
TaskHub is a lightweight, developer-friendly Task Management API built using Golang.
It helps you create, update, delete, and track tasks with simple, clean REST APIs — perfect for learning backend concepts or powering small productivity tools.

![Status](https://img.shields.io/badge/status-active-brightgreen) ![Node](https://img.shields.io/badge/node-%3E%3D16.0.0-blue) ![License](https://img.shields.io/badge/license-MIT-yellow)

## 🗳️Project Overview
TaskHub lets you create, read, update, and delete tasks like a productivity wizard.  
It’s simple, clean, and built with Go — meaning it runs fast enough to make your Java backend cry.

## ⚙️ Prerequisites
Before you summon the backend gods, make sure you have:
- Golang ≥ 1.20 (Go old or go home)
- MongoDB (local or Atlas — whichever crashes less for you)
- A .env file with:
```
PORT=4300
MONGO_URI=mongodb://localhost:27017/taskhub
```

## 🚀 Setup Instructions
```
# 1️⃣ Clone the repository (flex optional)
git clone https://github.com/your-username/taskhub-go.git

# 2️⃣ Enter the dungeon
cd taskhub-go

# 3️⃣ Summon the dependencies
go mod tidy

# 4️⃣ Start the magic
go run main.go
```
Your server will appear at:
```
http://localhost:4000
```

## 🔌 API Usage
Some sample spells from the TaskHub grimoire:
---
### 📘 GET /tasks
Retrieve all tasks — aka "What mess have I created?"

#### Response
```
[
  {
    "id": "6791ab991f",
    "title": "Write documentation",
    "status": "pending",
    "createdAt": "2025-01-01T10:00:00Z"
  }
]
```
---
### ➕ POST /tasks
Create a shiny new task.

#### Response
```
{
  "id": "6791ac2299",
  "title": "Learn Go",
  "status": "pending",
  "message": "Task created successfully!"
}
```

## 🚫 Troubleshooting
##### MongoDB connection error?
Don’t panic. Yet.
- Check if MongoDB is running
- If using Atlas, whitelist your IP, your house, and maybe your neighbor’s house too
- Verify your connection string isn’t cursed

##### Port already in use?
Change it in .env:
```
PORT=5000
```

## 🤙 Contributing
We love contributions almost as much as Go loves strict typing.

**Steps**:
1. Fork the repo
2. Make a branch
3. Commit cool stuff
4. Open a Pull Request
5. Bask in glory

## ⭐ Extras
--
#### 📁 Project Structure
```
taskhub-go/
 ├─ controllers/      # Where the magic happens
 ├─ models/           # Your data-shaped children
 ├─ routes/           # Your API’s front door
 ├─ database/         # MongoDB handshake logic
 ├─ utils/            # Helpers because you deserve happiness
 ├─ main.go
 └─ README.md
```

## 🐵 Issues
If my code sucks, please open an issue and let me know!

<img src="https://media1.giphy.com/media/v1.Y2lkPTc5MGI3NjExdXF4OHY5ZDQydmF2NjloajN4MDZoeWJ6NGE1dmJnZzVhb2RhdTdkcyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/Y1ybQjHgteZLa/giphy.webp" height="65" alt="Buzz GIF" title="Buzz GIF">

#### Like the work? 😍

Consider giving the repository a ⭐️  or [Buy Me A Coffee]()
