# nginx-fluentd-logging
## Prerequisites
- Docker
- Docker Compose
## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/nginx-fluentd-logging.git
   cd nginx-fluentd-logging
   ```sh
2. Start the containers:
   ```sh
   docker-compose up -d
   ```sh
## Viewing Logs
1. To check Fluentd logs:
   ```sh
   docker-compose logs -f fluentd
   ```sh
2. To check Nginx logs:
   ```sh
   docker-compose logs -f nginx
   ```sh
## Stopping the Services
```sh
docker-compose down
```sh
