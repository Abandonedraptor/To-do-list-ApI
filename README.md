# 🧩 To-Do API (Flask + Docker)

A simple yet powerful **Flask REST API** for managing to-do items.  
Built with clean architecture, containerized with Docker, and designed as a portfolio sample for **API & Software Development**.

---

## 📖 Overview

This project demonstrates:
- ✅ Flask-based REST API design  
- 🧠 SQLite database integration  
- ⚙️ Docker & Docker Compose setup  
- 🚀 Ready-to-deploy environment for development or production  

---

## 🧱 Features

- Create, read, update, and delete to-do items
- Lightweight SQLite storage
- Fully containerized with Docker
- Auto-reload in development mode
- Clean, beginner-friendly code structure

---

## 📁 Project Structure

todo-api-flask/
│
├── app/
│ ├── init.py
│ ├── models.py
│ ├── routes.py
│ └── database.db
│
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
├── run.py
└── README.md
---

## 🐳 Run with Docker (Recommended)

> Requires: [Docker](https://docs.docker.com/get-docker/) and [Docker Compose](https://docs.docker.com/compose/install/)

1. **Clone the repository**
   ```bash
   git clone https://github.com/<your-username>/todo-api-flask-docker.git
   cd todo-api-flask-docker
Build and start the container
docker-compose up --build
Visit the API
👉 http://localhost:5000

Stop the container
docker-compose down
Your data is stored in a Docker volume named sqlite_data.
🧑‍💻 Run Locally (Without Docker)

Requires Python 3.10+ installed.

Clone the repo
git clone https://github.com/<your-username>/todo-api-flask-docker.git
cd todo-api-flask-docker
Set up virtual environment
python -m venv venv
source venv/bin/activate      # macOS/Linux
venv\Scripts\activate         # Windows
Install dependencies
pip install -r requirements.txt
Run the app
flask run
Then open 👉 http://127.0.0.1:5000
🔗 API Endpoints
| Method | Endpoint      | Description           |
| ------ | ------------- | --------------------- |
| GET    | `/todos`      | Get all to-dos        |
| GET    | `/todos/<id>` | Get a single to-do    |
| POST   | `/todos`      | Create new to-do      |
| PUT    | `/todos/<id>` | Update existing to-do |
| DELETE | `/todos/<id>` | Delete to-do          |
🧩 Example Request
curl -X POST http://127.0.0.1:5000/todos \
     -H "Content-Type: application/json" \
     -d '{"title": "Learn Docker", "done": false}'
Response:
{
  "id": 1,
  "title": "Learn Docker",
  "done": false
}
👨‍💻 About the Developer

Kevin Orina Obiero
Software Engineer & API Developer
📧 obierokevin83@gmail.com
⭐ If you found this useful, don’t forget to star the repo!
