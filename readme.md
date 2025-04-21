# 🚀 MySQL + phpMyAdmin with Docker Compose

This project sets up a MySQL database with phpMyAdmin using Docker Compose. It's a quick and easy way to get a local MySQL environment with a web-based UI for managing your databases.

## 🧱 Stack

- **MySQL 8.0**
- **phpMyAdmin**
- **Docker & Docker Compose**

## 📦 Requirements

- Docker Desktop (Windows, macOS, or Linux)
- Docker Compose (built into Docker Desktop)

## 📁 Folder Structure

. ├── docker-compose.yml 
  └── README.md

## ⚙️ Setup

1. Clone this repository:
   git clone https://github.com/heinthant/docker-mysql-phpmyadmin.git
   cd docker-mysql-phpmyadmin
Start the containers:

docker-compose up -d
Access phpMyAdmin at:http://localhost:8080

🔐 Default Credentials

Property	Value
MySQL Root User	root
MySQL Root Password	rootpassword
MySQL User	user
MySQL User Password	userpassword
MySQL Database	mydb
You can change these in the docker-compose.yml file as needed.

🗃️ Data Persistence
MySQL data is stored in a Docker volume named mysql_data.

Data will persist between container restarts.

🛑 Stopping Everything
To stop and remove the containers:

docker-compose down
🧼 Remove All Data (Optional)
If you want to delete the MySQL data volume too:

docker-compose down -v
🧠 Notes
Make sure Docker Desktop is running and you're using Linux containers.

You can modify or extend this setup by adding PHP, Apache, or other services as needed.

📄 License
MIT License