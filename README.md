# Binance-Trading-Bot

This is my first try of a Trading Bot for Binance. We will use the RSI for our sell and buy decisions for Ethereum.

## Table of Contents

* [DISCLAIMER](#disclaimer)
* [General Info](#general-info)
* [Technologies](#technologies)
* [Setup](#setup)
* [Docs](#docs)
* [Author](#author)

## DISCLAIMER
This project is for educational purpose!
I am not responsible for the trades you make with the script, this script has not been exstensivly tested on live trades.
## General Info
I always wanted to code my own Trading Bot. I found a lot of information for the Binance API on the web, so I thought
I would give it a shot. Also, I wanted to learn to use websockets with Phython.

The trading strategy I used for this project is based on the RSI (Relative Strength Index). Basically, we will calculate 
the RSI with the 14 recent close values. If the RSI is over 70 we will sell or Assets, because the market is overbought.
And when the RSI is lower than 30 we will buy ETH, because the market is oversold. For more information visit: [Wikipedia-RSI](https://en.wikipedia.org/wiki/Relative_strength_index)

## Technologies
The Project is created with:

* Python 3.7
* TA-Lib 0.4.19
* Numpy 1.19.4
* Python-binance 0.7.5
* Websocket-client 0.57.0

## Setup

1. [Signup](https://www.binance.com/de/register?ref=58495589) for Binance
2. Go to the API Center and create a new API key
```
[✓] Read Info [✓] Enable Trading [X] Enable Withdrawals
```

3. Insert your key and secret into ``config.py``


To install all libs run following command:

```
pip install requirements
```

## Docs

* [Binance API](https://python-binance.readthedocs.io/en/latest/binance.html)
* [Websocket-Stream](https://github.com/binance-exchange/binance-official-api-docs/blob/master/web-socket-streams.md)


## Author
Stefan Helm

