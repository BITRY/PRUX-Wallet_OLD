PRUX COIN  

SPEC.:

Hash Algorithm : Scrypt

Typ : Proof-of-Work

Block Time : 9sec

Miner Reward : 0.00959499 PRUX

Mined Block Confirmation : 274

Premine = ZERO


::::::::::::::::::::::::::::::::::::::::::::::::BUILD WALLET INSTRUCTION::::::::::::::::::::::::::::::::::::::::::::::::::::::::


LINUX / UBUNTU 14.04 BUILD READ FILE HERE -------->>>>  /prux/doc/build-unix.txt

START WITH

./prux-qt -server -addnode=80.218.217.199:9595

or

./prux -server -addnode=80.218.217.199:9595


POOL LIST 
https://yiimp.mastermining.net/site/mining
http://www.bitcoin-pool.de


EXCHANGE
https://tradesatoshi.com/Exchange/?market=PRUX_BTC 

===========

[![Build Status](https://*************.png?branch=master)](https:/***********/prux)





UBUNTU 14.04 BUILD NOTES
========================

sudo add-apt-repository ppa:bitcoin/bitcoin
sudo apt-get update
sudo apt-get install qt4-dev-tools libqt4-dev libqt4-core libqt4-gui
sudo apt-get install build-essential
sudo apt-get install libssl-dev
sudo apt-get install libdb4.8-dev if not work try sudo apt-get install libdb-dev
sudo apt-get install libdb4.8++-dev  if not work try sudo apt-get install libdb++-dev
sudo apt-get install libqrencode-dev
sudo apt-get install libboost1.48-dev   if not work try  sudo apt-get install libboost-dev
sudo apt-get install libboost1.48-all-dev  if not work try  sudo apt-get install libboost-all-dev

BUILD
=====

cd PRUX-COIN-master
qmake "USE_UPNP=-"
make                        (or  make -j2  , 2 core or the fast way or turbo with -j8)

cd src
make -f  makefile.unix USE_UPNP=-      (or -j2  ,the fast way or turbo with -j8)


if error can help
cd src
chmod +x leveldb/build_detect_platform
again


Running
=====

/src/./prux 

or QT-Wallet

/./prux-qt -server







