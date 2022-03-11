# Dockerfiles for ssh

docker build -t <image_tag> . <- this is where your dockerfile is

docker run -d -P --name <container_name> <image_tag>

docker inspect --format='{{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}' <container_name>

ssh root@Ip-of-above-command
