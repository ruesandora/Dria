# Dria

> Mevcut sunucularımdan birinde run ediyorum.

> Boş duran sunucuyu Allah sevmez, beklentisiz runladım.

## Kurulum

```console

# güncelleme ve docker kurulumu
sudo apt update && sudo apt upgrade -y

for pkg in docker.io docker-doc docker-compose docker-compose-v2 podman-docker containerd runc; do sudo apt-get remove $pkg; done

#

sudo apt-get update
sudo apt-get install ca-certificates curl
sudo install -m 0755 -d /etc/apt/keyrings
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
sudo chmod a+r /etc/apt/keyrings/docker.asc

#

echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
  $(. /etc/os-release && echo "$VERSION_CODENAME") stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

sudo apt-get update

#

sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
sudo docker run hello-world
```

#

```console
# Dria kurulumu

git clone https://github.com/firstbatchxyz/dkn-compute-node
cd dkn-compute-node

cp .env.example .env
nano .env
#
```

> `.env` içersinde testnet `metamaskımızın private keyini` ve `openAI API key` ekliyoruz.

> `DKN_WALLET_SECRET_KEY` kısmına `Private keyi`

> `OPENAI_API_KEY=` kısmına [buradan](https://platform.openai.com/api-keys) key alıp

```console
screen -S Dria

sudo systemctl start docker

chmod +x start.sh

./start.sh -m=llama3.1:latest -m=gpt-3.5-turbo
```

> CTRL A D İLE ÇIKALIM

> Ana screende loglara bakalım.

> `docker compose logs -f compute`

<img width="957" alt="Ekran Resmi 2024-08-20 00 47 23" src="https://github.com/user-attachments/assets/28f3a3a7-d4e6-4dec-96a0-6d38bc69d419">


> Çıktı böyleyse tebrikler.

> Formuda dolduralım [buradan](https://docs.google.com/forms/u/0/d/e/1FAIpQLSeK090ejc4dg5x1ztb_yAOxGz5o1V8JUqDa-o3AwV1Lq7NpMA/formResponse?pli=1)

<img width="485" alt="Ekran Resmi 2024-08-20 00 48 00" src="https://github.com/user-attachments/assets/bbc4f110-6956-48c7-90b4-f891be0809fd">

> [Discord](https://discord.gg/utj2k7V8)



