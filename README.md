# taiko-node-guide
This is a scription to guide you run a taiko node
sudo apt update

sudo apt install git

sudo apt install apt-transport-https ca-certificates software-properties-common curl

sudo curl -f -s -S -L https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu bionic stable"

cd /root

sudo apt install docker-ce docker-ce-cli containerd.io docker-compose-plugin -y

sudo systemctl status docker

git clone https://github.com/taikoxyz/simple-taiko-node.git

cd simple-taiko-node

cp .env.sample .env

docker compose up

