# spring-boot-micrometer
Spring Boot Actuator metrics monitoring with Prometheus and Grafana

1) PULL docker images Prometheus and Grafana form docker hub registry :

2) For prometheus image to container running command :
docker run -p 9090:9090 -v C:\Users\ASUS\Pictures\TWS\Git\Spring-pratice\spring-boot-micrometer\src\main\resources\prometheus.yml prom/prometheus

NOTE : The command you provided is a Docker command to run a Prometheus instance. It has the following options:

    -p 9090:9090: This option maps the Prometheus port 9090 to the host port 9090.
    -v C:\Users\ASUS\Pictures\TWS\Git\Spring-pratice\spring-boot-micrometer\src\main\resources\prometheus.yml:/prometheus.yml: This option mounts the Prometheus configuration file (prometheus.yml) from the host to the container.
    prom/prometheus: This is the image name of the Prometheus container.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

3) For Grafana image to container running command :

The following Docker command will run a Grafana container in the background, map port 3000 on the host machine to port 3000 in the container, and name the container "grafana":

docker run -d -p 3000:3000 --name=grafana grafana/grafana

The following are the options used in the command:

    -d: Runs the container in the background.
    -p 3000:3000: Maps port 3000 on the host machine to port 3000 in the container.
    --name=grafana: Names the container "grafana".
    grafana/grafana: Specifies the Grafana Docker image.
