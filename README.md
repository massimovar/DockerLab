# Docker Container Stack for Monitoring and Management

This stack deploys a collection of Docker containers for managing and monitoring data, ideal for development and testing in IoT, analytics, and server administration.

## Services

1. Portainer:
   - Purpose: Docker management tool with web UI.
   - Access: <https://localhost:9443>

2. InfluxDB:
   - Purpose: Time-series database for storing metrics.
   - Access: Accessible on localhost:8086

3. Chronograf:
   - Purpose: Visualization tool for InfluxDB data.
   - Access: Accessible on localhost:8888

4. MySQL:
   - Purpose: Relational database for structured data.
   - Access: Default port 3306 (MySQL clients or phpMyAdmin).

5. phpMyAdmin:
   - Purpose: Web interface for MySQL management.
   - Access: <http://localhost:8080>

6. MQTT Broker:
   - Purpose: Message broker for IoT communication (Mosquitto).
   - Access: MQTT on localhost:1883, WebSocket on localhost:9001

7. Prometheus:
   - Purpose: Metrics collection and monitoring.
   - Access: Accessible on localhost:9090

8. Grafana:
   - Purpose: Visualization tool for Prometheus and InfluxDB data.
   - Access: <http://localhost:3001>

## Usage

1. Clone the repository.
2. Run install_docker.sh to install Docker and Docker Compose.
3. Use docker-compose up -d to start the containers.
4. Access each service via the provided URLs for setup and usage.

## Notes

- Network: All containers share the same monitoring network for easy intercommunication.
- Data Persistence: Volumes are defined to store persistent data for InfluxDB, MySQL, Prometheus, and Grafana.

Enjoy monitoring and managing with this Docker stack!
