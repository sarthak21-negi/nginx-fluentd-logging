# nginx-fluentd-logging
## Prerequisites
- Docker
- Docker Compose
## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/nginx-fluentd-logging.git
   cd nginx-fluentd-logging
   
2. Start the containers:
   ```sh
   docker-compose up -d
   
## Viewing Logs
1. To check Fluentd logs:
   ```sh
   docker-compose logs -f fluentd
   
2. To check Nginx logs:
   ```sh
   docker-compose logs -f nginx
   
## Stopping the Services
```sh
docker-compose down

