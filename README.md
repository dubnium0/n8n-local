# How to Run n8n, Postgres, and pgAdmin with Docker

This project lets you easily run n8n (automation tool), Postgres (database), and pgAdmin (database manager) using Docker.

## Requirements

- [Docker](https://www.docker.com/products/docker-desktop) installed
- [Docker Compose](https://docs.docker.com/compose/) (comes with Docker Desktop)

## Getting Started

1. **Go to Your Project Folder**

   Open your terminal or PowerShell and go to the folder where this file is:
   ```sh
   cd c:\Users\ahmet\Desktop\n8n-local
   ```

2. **Start the Services**

   Run this command to start everything:
   ```sh
   docker-compose up -d
   ```

   This will start n8n, Postgres, and pgAdmin in the background.

3. **Access the Apps**

   - **n8n:**  
     Open [http://localhost:5678](http://localhost:5678)  

   - **pgAdmin:**  
     Open [http://localhost:8080](http://localhost:8080)  
     Email: `admin@admin.com`  
     Password: `admin123`

   - **Postgres Database Info:**  
     - Host: `postgres`
     - Port: `5432`
     - Database: `n8ndb`
     - User: `n8n`
     - Password: `n8npassword`

## Notes

- Your data is safe because Docker volumes are used.
- You can change usernames, passwords, and other settings in the `docker-compose.yml` file.
