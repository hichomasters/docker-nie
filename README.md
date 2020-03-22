NiceHash CPU Mining Container
=============================

A simple docker container image for the nheqminer Equihash miner.

https://github.com/nicehash/nheqminer

There are 4 ENVIRONMENT variables to configure (shown here with defaults):

    BTC_PAYMENT_ADDRESS=3DU6hoKdFtwtSiekFAszpv6Np9Undcg9dW
    BTC_THREADS=8
    BTC_WORKER_ID=`hostname`
    BTC_SERVER=equihash.usa.nicehash.com:3357

Eg.

    docker service create --mode global \
      --name nicehash-miner \
      -e BTC_PAYMENT_ADDRESS=3DU6hoKdFtwtSiekFAszpv6Np9Undcg9dW \
      idstudios/nicehash-miner:latest

Example JSON configurations for DC/OS illustrate usage.
