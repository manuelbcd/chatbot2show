# chatbot2show


## Development

### Steps

1. Prepare min. ubuntu server >= 14.04
2. Install go lang
```
wget https://dl.google.com/go/go1.10.3.linux-amd64.tar.gz
sudo tar -C /usr/local -xvf go1.10.3.linux-amd64.tar.gz
echo "export GOPATH=$HOME/go" >> ~/.bash_profile
echo "export PATH=$PATH:/usr/local/go/bin:$GOPATH/bin" >> ~/.bash_profile
source ~/.bash_profile
mkdir ~/go/src
cd ~/go/src
git clone https://github.com/target/flottbot.git
cd ~/go/src/flottbot/cmd/flottbot
go get
```
3. Set go paths

## Execution

### Quick start

```
docker run -it --rm --name mybot -v "$PWD"/config:/config target/flottbot:latest /bin/sh -c "./flottbot"
```

### Docker-compose
```
docker-compose up -d
```

## Useful information

flottbot repo https://github.com/target/flottbot

flottbot doc  https://target.github.io/flottbot-docs/basics/quick-start/

dareCode https://darecode.com
