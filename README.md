WordPress + MySQL Using Docker Compose

This project deploys a fully containerized WordPress + MySQL stack using Docker Compose.
It includes:

WordPress container (Apache + PHP)

MySQL 5.7 database container

Persistent Docker volumes

Internal service networking

Environment variable–based configuration

Perfect for DevOps learning, POCs, and reproducible development environments.

Project Structure
wordpress-docker/
├── docker-compose.yml
├── .env
└── README.md

 How to Run the Project
1. Clone the Repository
git clone https://github.com/yourusername/wordpress-docker.git
cd wordpress-docker

2. Start the Containers
docker-compose up -d

3. Check Running Containers
docker ps


You should see wordpress and mysql.

 Access WordPress

Open your browser:

http://localhost:8080


If deployed on a server:

http://YOUR_SERVER_IP:8080


You will see the WordPress installation page.

 Stop the Stack
docker-compose down


Remove volumes:

docker-compose down -v

 Environment Variables

Located in .env:

WORDPRESS_DB_USER=wpuser
WORDPRESS_DB_PASSWORD=wppassword123
WORDPRESS_DB_NAME=wordpress
MYSQL_ROOT_PASSWORD=rootpass123

 Technologies Used

Docker

Docker Compose

WordPress

MySQL 5.7

Linux

Shell



 License

MIT License.
