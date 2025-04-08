**🔹 You can access Gensyn Node Step-by-Step YouTube Guide from here: https://youtu.be/cIsVKOku5Ow**

**🚀Credit:** Gensyn Node Guide is created by ZUN, I have adjusted Acc to own style so that my community can easily join the Gensyn testnet.

**❤️❤️Follow our TG for More Early Alpha: https://telegram.me/feature_earning**

## Install Dependencies
**. Update System Packages**
```bash
sudo apt-get update && sudo apt-get upgrade -y
```
**. Install Node.js and npm**
```console
curl -sSL https://raw.githubusercontent(.)com/zunxbt/installation/main/node.sh | bash
```
 **.Install other dependencies using the command below**
 ```console
sudo apt update && sudo apt install -y python3 python3-venv python3-pip curl screen git yarn && curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add - && echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list && sudo apt update && sudo apt install -y yarn
```
**. Clone this repository**

```console
rm -rf rl-swarm && git clone https://github.com/zunxbt/rl-swarm.git && cd rl-swarm
```
**. Create a screen session**

```console
screen -S gensyn
```
**. Run the swarm**

```console
python3 -m venv .venv && source .venv/bin/activate && ./run_rl_swarm.sh
```
