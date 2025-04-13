# Gensyn-Testnet
Process to run Gensyn testnet 
ssh -p 2092 root@n1.us.clorecloud.net
ssh -p 2092 root@n1.de.clorecloud.net



apt update && apt install -y telnet && telnet 38.101.215.13 30111

apt install curl -y

curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.2/install.sh | bash

\. "$HOME/.nvm/nvm.sh"

nvm install 22

node -v

nvm current

corepack enable yarn

yarn -v

apt install -y python3.12-venv

git clone https://github.com/gensyn-ai/rl-swarm.git


screen -S gensyn

cd rl-swarm/

sed -e 's/2.20.0/2.25.0/g' modal-login/package.json

sed -i -e 's/2.20.0/2.25.0/g' modal-login/package.json

python3 -m venv .venv

source .venv/bin/activate

pip install colorlog

./run_rl_swarm.sh

Daemon Error:
sed -i -E 's/(startup_timeout: *float *= *)[0-9.]+/\1120/' $(python3 -c "import hivemind.p2p.p2p_daemon as m; print(m.__file__)")

./run_rl_swarm.sh
