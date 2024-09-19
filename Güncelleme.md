
## Dria Güncelleme
```console
screen -r Dria
Çalışan servis varsa ctrl+c ile durduralım


öncelikle DKN_WALLET_SECRET_KEY i ve OPENAI_API_KEY i bir yere not edin
```console
nano ~/dkn-compute-node/.env

```console
rm -rf dkn-compute-node

# güncelleme 
```console
sudo apt update && sudo apt upgrade -y



```console
# Dria kurulumu
curl -L -o dkn-compute-node.zip https://github.com/firstbatchxyz/dkn-compute-launcher/releases/latest/download/dkn-compute-launcher-linux-amd64.zip
unzip dkn-compute-node.zip
cd dkn-compute-node

nano .env
#
```
> `.env` içersinde testnet `DKN_WALLET_SECRET_KEY i ve OPENAI_API_KEY i` ekliyoruz.
ctrl+x y enter ile çıkalım


```console
ollama pull hellord/mxbai-embed-large-v1:f16


```console
./dkn-compute-launcher -m=llama3.1:latest -m=gpt-4o-mini
```

> CTRL A D İLE ÇIKALIM



> [Discord](https://discord.gg/utj2k7V8)



