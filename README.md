<p align="center"><img height="100" height="auto" src="https://github.com/furidngrt/subsquid/assets/63885192/5bffb1ea-3f82-4bf7-8035-fd99781c630f)](https://github-production-user-asset-6210df.s3.amazonaws.com/63885192/275373993-5bffb1ea-3f82-4bf7-8035-fd99781c630f.png"></p>

 Subsquid is a data network designed for the future of Web3: rapidly and cost-efficiently retrieve blockchain data from 100+ chains using Subsquid’s decentralized data lake and open-source SDK to build billion-user dApps.

### Install Git :
```
sudo apt update
```

```
sudo apt install git
```

### Install Nodejs

```
sudo apt install nodejs
```

```
sudo apt install npm
```

```
npm install -g npm@10.2.0
```

### Install Docker

```
sudo apt-get install ca-certificates curl gnupg lsb-release -y
```

```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```

```
sudo apt-get update
```

```
sudo apt-get install docker-ce docker-ce-cli containerd.io -y
```

### Install Subsquid

```
mkdir global-node-packages
npm config set prefix ~/global-node-packages
export PATH="${HOME}/global-node-packages/bin:$PATH"
```

```
cd global-node-packages
npm install --global @subsquid/cli@latest
```

```
sqd init newfolder -t https://github.com/subsquid-quests/single-chain-squid
cd newfolder
```


in the Subsquid Web Task Retrieve Key File > Click Get Key > Upload File in Folder `/query-gateway/keys`


```
sqd up
```

```
npm ci
```

```
sqd build
```

```
sqd migration:apply
```

```
sqd run .
```

wait about 20 minutes for the claim button to appear on the web task.

```
sqd down
```


## Run Network Test One

```
sudo apt update
sudo apt install git
```

### NodeJs

```
sudo apt install nodejs -y
sudo apt install npm -y
npm install -g npm@10.2.1
```

### Docker

```
sudo apt-get install ca-certificates curl gnupg lsb-release -y
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io -y
```

### install

```
mkdir global-node-packages
npm config set prefix ~/global-node-packages
export PATH="${HOME}/global-node-packages/bin:$PATH"
```
```
cd global-node-packages
npm install --global @subsquid/cli@latest
```
```
sqd init uniform-load-squid -t https://github.com/subsquid-quests/network-test-one-uniform-load-squid
cd uniform-load-squid
npm ci
```

```
sqd get-peer-id
```

```
sqd up
sqd build
sqd run .
```

