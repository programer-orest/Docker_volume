Dockerizing Django-Todolist with MySQL and Volumes
📌 Project Overview
This project demonstrates how to containerize a Django Todo-List web application with a MySQL database using Docker.
The main focus was on creating a persistent MySQL container with attached volumes and connecting the Django application container to the MySQL container.

🛠 Tech Stack
Docker

MySQL (official Docker image)

Django (Python framework)

Docker Hub (for image storage)

🚀 What Was Done
1. Created Dockerfile.mysql to build a custom MySQL image based on the official MySQL Docker image.

2. Configured environment variables to initialize:

  - Database: app_db

  - User: app_user

  - Password: 1234

3. Built a MySQL Docker image tagged as mysql-local:1.0.0.

4. Created and attached Docker volumes to persist MySQL data outside the container.

5. Pushed the MySQL image to a personal Docker Hub repository.

6. Run the MySQL container locally with attached volumes.

7. Updated Django app database configuration to connect to the running MySQL container’s IP.

8. Built and ran the updated Django app container connected to the MySQL database.

9. Pushed the Django app image to Docker Hub with the tag todoapp:2.0.0.

10. Created INSTRUCTION.md with detailed steps for running both MySQL and Django app containers, including:

- Volume mounting

- Access instructions
