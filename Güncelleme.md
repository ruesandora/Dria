
## Dria Güncelleme
```console
screen -r Dria
```
>Çalışan servis varsa ctrl+c ile durduralım


>öncelikle DKN_WALLET_SECRET_KEY i ve OPENAI_API_KEY i bir yere not edin
```console
nano ~/dkn-compute-node/.env
```

```console
rm -rf dkn-compute-node
```

# güncelleme 
```console
sudo apt update && sudo apt upgrade -y
```
# Ollama kurulumu
```console
curl -fsSL https://ollama.com/install.sh | sh
```

# Dria kurulumu
```console
curl -L -o dkn-compute-node.zip https://github.com/firstbatchxyz/dkn-compute-launcher/releases/latest/download/dkn-compute-launcher-linux-amd64.zip
unzip dkn-compute-node.zip
cd dkn-compute-node
```

> `.env` içersinde testnet `DKN_WALLET_SECRET_KEY i ve OPENAI_API_KEY i` ekliyoruz.
```console
nano .env
```
>ctrl+x y enter ile çıkalım

> Dria yı çalıştırıyoruz
```console
ollama pull hellord/mxbai-embed-large-v1:f16
```
```console
./dkn-compute-launcher -m=llama3.1:latest -m=gpt-4o-mini
```
> Komutu girdikten sonra 2 defa enter e basıyoruz, bazı paketleri kontrol ediyor ve indirme işlemi yapıyor çalışmaya başlaması biraz zaaman alabilir

> CTRL A D İLE ÇIKALIM







