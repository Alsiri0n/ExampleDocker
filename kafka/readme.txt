Required to host machine in hosts file
192.168.1.2 kafka.lan
With correct ip address

Documentation for apache kafka
https://kafka.apache.org/documentation/

Run no-auth container
docker compose -f compose.yml -f compose.no-auth.yml up -d
podman compose -f compose.yml -f compose.no-auth.yml up -d
