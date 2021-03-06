# Tweet Activated Crypto Trader

### Feb 10th 2021 - Working, has been tested on DOGE/BTC (Kraken & Binance), DOGE/GBP (Binance), successfully made a 17% return from Elon's latest Doge tweet

The idea is to buy crypto using a Twitter trigger and sell after a user specified time / price / % gain e.g. when Elon musk tweets about Dogecoin

Markets, particularly small market cap altcoins are heavily influenced by individuals with large following 'hyping' up a cryptocurrency, crypto pumps. We can capitalize on this opportunity by being one of the first to exectue trades when a tweet is posted

When a Tweet is posted, it checks for substring matches with keywords for a particularcryptpcurrency, these keywords can be edited and more cryptos can be added in order to execute the trade

To run with Binance: `python twitter_binance.py`, to run with Kraken: `python detect_tweet.py` API keys are kept in a json called one directory up from repo ../keys.json

## To Do
- Backtest (done)
- User input parameters (done)
- Error handling if trade is unclosed (done)
- Fully implement Binance (lower taker/maker fees - 0.01% compared to Krakens 0.26%) (done)
- Trade logging json mechanism
- Verify working on BTC
- Reduce latency between tweet and trade from 3s to <1s
- Get a list of accounts to follow
- Test for multiple other cryptos/alt coins
- Mechanism for pulling out of all positions
- Limit orders
- Implement sentiment feature for size of position or whether to short (potentially object detection)


## Notes
- Requires a Twitter Developer API detecting tweets through Tweepy
- Requires a crypto exchange (Kraken/Binance) API which is used through ccxt
	- Uses ccxt (cryptocurrency exchange trading library which has support for a huge number of exchanges and APIs)





