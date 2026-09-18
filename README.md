curl -fsSL <https://get.docker.com> -o get-docker.sh
sudo sh get-docker.sh

sudo systemctl is-active docker
sudo docker --version
sudo docker compose version