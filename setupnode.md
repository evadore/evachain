### For example setup.sh
sudo DEBIAN_FRONTEND=noninteractive DEBIAN_PRIORITY=critical apt install ntpdate

sudo DEBIAN_FRONTEND=noninteractive DEBIAN_PRIORITY=critical ntpdate -s time.nist.gov

sudo DEBIAN_FRONTEND=noninteractive DEBIAN_PRIORITY=critical sudo apt-get update -y

sudo DEBIAN_FRONTEND=noninteractive DEBIAN_PRIORITY=critical sudo apt-get upgrade -y

sudo DEBIAN_FRONTEND=noninteractive DEBIAN_PRIORITY=critical sudo add-apt-repository -y ppa:ethereum/ethereum

sudo DEBIAN_FRONTEND=noninteractive DEBIAN_PRIORITY=critical sudo apt-get install ethereum -y

sudo DEBIAN_FRONTEND=noninteractive DEBIAN_PRIORITY=critical sudo apt-get -y upgrade geth 

sudo DEBIAN_FRONTEND=noninteractive DEBIAN_PRIORITY=critical sudo apt-get install solc -y

cd /home

mkdir cdata

sudo geth --datadir /home/cdata init evachain.json
