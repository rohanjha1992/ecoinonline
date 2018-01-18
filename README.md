ecoinonline (ECE) is a digital decentralised currency crafted by Genius Marketers involving Blockchain Technology

Installation
===========================

The installation requires at least a VPS having 2 GB OF RAM, 2 CORE CPU AND 40GB HDD with UBUNTU 16.04 installed on it. 

Steps:
 
1) Update your Ubuntu 16.04 machine.

sudo apt-get update

sudo apt-get upgrade

2) Install the dependencies to compile from source code.

sudo apt-get install build-essential libssl-dev libdb++-dev git libssl1.0.0-dbg libdb-dev libboost-all-dev libminiupnpc-dev libevent-dev libcrypto++-dev libgmp3-dev 

3) Download source code from repository.

git clone https://github.com/rohanjha1992/ecoinonline.git

4) Go to the src directory of your coin.

cd ecoinonline/src

5)  Make build_detect_platform is executable.

chmod +x leveldb/build_detect_platform

6) Execute the following command to compile the daemon.

make -f makefile.unix RELEASE=1

7) Run the Coin Server using ./ecoinonlined command

You will see message to create username and password

8) Create a new configuration file.

sudo nano /root/.ecoinonline/ecoinonline.conf

9) Paste the following lines in ecoinonline.conf file and save it.

rpcuser=rpc_ecoinonline

rpcpassword=yourrandompassword

rpcallowip=127.0.0.1

listen=1

server=1

txindex=1

daemon=1

10) Run the Coin Server using ./ecoinonlined command

RPC port	21264

P2P port	21263

List of API call list can be found here : https://en.bitcoin.it/wiki/Original_Bitcoin_client/API_calls_list

For any kind of installation issue email at : info@ecoinonline.org