# Task 7: Monitor System Resources Using Netdata

## Objective

Install Netdata using Docker and visualize system and application performance metrics.

## Tools Used

- Docker
- Netdata (official image: `netdata/netdata`)
- VS Code
- GitHub

## Steps Performed

1. Ran Netdata container using:

docker run -d --name=netdata -p 19999:19999 netdata/netdata

2. Verified container status with `docker ps`
3. Accessed dashboard at `http://localhost:19999`
4. Explored metrics: CPU, memory, disk I/O, Docker containers
5. Reviewed alerts and logs using:

docker exec -it netdata cat /var/log/netdata/error.log

6. Captured screenshot of live dashboard

## Screenshot

![Netdata Dashboard](task-7-netdata-dashboard.png)

## Outcome

Gained hands-on experience with lightweight system monitoring using Netdata. Learned how to visualize real-time metrics and interpret alerts for system health.
