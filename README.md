# nginx-fluentd-logging

## Why chose fluentd
I chose Fluentd as my logging solution because it is lightweight, easy to use, and works well with containers like Docker. Fluentd connects directly with NGINX using a simple configuration (access_log fluentd:24224), so I don’t need to install extra tools to collect logs. It also stores logs in a structured format (JSON), which makes them easier to read, search, and analyze. This helps us quickly understand what’s happening with our NGINX server without complicated setups.
## Why I didn't chose other logging solution
Other logging solutions like Filebeat, Logstash, Promtail, Graylog, OpenSearch, Rsyslog, Vector, and ClickHouse were not chosen because they require more setup and are better suited for larger, more complex systems. Filebeat is mainly designed to read logs from files rather than directly collecting logs from NGINX. Logstash, while powerful, is resource-heavy and not ideal for a lightweight demo. Promtail is primarily focused on Kubernetes environments rather than standalone NGINX setups.

Graylog and OpenSearch need extra servers to store and process logs, making them too complex for this demo. Rsyslog is older and better suited for traditional system logs rather than modern container setups. Vector is a newer option but not widely used for NGINX logging. ClickHouse is fast for storing logs but requires extra setup for processing and queries. Fluentd stands out because it integrates easily with NGINX, making log collection simple and efficient.

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

