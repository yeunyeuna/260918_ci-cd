curl -fsSL <https://get.docker.com> -o get-docker.sh
sudo sh get-docker.sh

sudo systemctl is-active docker
sudo docker --version
sudo docker compose version


pbcopy < ./"$MY_KEY_NAME".pem 2>/dev/null || xclip -selection clipboard < ./"$MY_KEY_NAME".pem 2>/dev/null || cat ./"$MY_KEY_NAME".pem
echo "SSH 키가 복사되었습니다. GitHub Secrets의 EC2_SSH_KEY 값에 붙여넣으세요."