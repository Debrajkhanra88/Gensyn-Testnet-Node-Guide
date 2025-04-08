**🔹 You can access Gensyn Node Step-by-Step YouTube Guide from here: https://youtu.be/cIsVKOku5Ow**

**🚀Credit:** Gensyn Node Guide is created by ZUN, I have adjusted Acc to own style so that my community can easily join the Gensyn testnet.

**❤️❤️Follow our TG for More Early Alpha: https://telegram.me/feature_earning**

## Install Dependencies
**1. Update System Packages**
```bash
apt update && apt install -y sudo
```
**2. Install General Utilities and Tools**
```bash
sudo apt update && sudo apt install -y python3 python3-venv python3-pip curl wget screen git lsof nano unzip
```

**3. Install Docker**
```bash
# Remove old Docker installations
for pkg in docker.io docker-doc docker-compose podman-docker containerd runc; do sudo apt-get remove $pkg; done

# Add Docker repository
sudo apt-get update
sudo apt-get install ca-certificates curl gnupg
sudo install -m 0755 -d /etc/apt/keyrings
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
sudo chmod a+r /etc/apt/keyrings/docker.gpg

echo \
  "deb [arch="$(dpkg --print-architecture)" signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
  "$(. /etc/os-release && echo "$VERSION_CODENAME")" stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

# Install Docker
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin

# Test Docker
sudo docker run hello-world
```
**4. Install Node.js and npm**
```console
curl -sSL https://raw.githubusercontent.com/FEdanish/Gensyn/refs/heads/main/node.sh | bash
```

**5. Clone this repository**

**6. Create a screen session**

```console
screen -S gensyn
```

**7. Run the swarm**

```console
python3 -m venv .venv && . .venv/bin/activate && ./run_rl_swarm.sh
```

