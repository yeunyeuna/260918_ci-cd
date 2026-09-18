sudo docker run -d \
--name watchtower-poll \
--restart unless-stopped \
-v /var/run/docker.sock:/var/run/docker.sock \
-e DOCKER_API_VERSION=1.44 \
containrrr/watchtower \
--interval 30 \
--cleanup \
app-blue