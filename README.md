# btc-race-24h-20261118-1444

[![make.fun · btc-race-24h-20261118-1444](https://make.fun/badge/btc-race-24h-20261118-1444.svg)](https://make.fun/bounty/btc-race-24h-20261118-1444?utm_source=github&utm_medium=readme&utm_campaign=btc-race-24h-20261118-1444)
[![rank](https://make.fun/badge/btc-race-24h-20261118-1444/Freshaaaa/btc-race-24h-20261118-1444/rank.svg)](https://make.fun/bounty/btc-race-24h-20261118-1444/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=btc-race-24h-20261118-1444)
[![reward](https://make.fun/badge/btc-race-24h-20261118-1444/Freshaaaa/btc-race-24h-20261118-1444/reward.svg)](https://make.fun/bounty/btc-race-24h-20261118-1444?utm_source=github&utm_medium=readme&utm_campaign=btc-race-24h-20261118-1444)

DipCatcher v2: a rare-trade oversold-dip catcher for cbBTC/USDC on 1-minute bars, built for make.fun's "Race a BTC trading bot live for 24 hours" bounty. It buys the whole equity only when RSI(30) drops below 20 *and* the close sits at least 1.2% under the 60-bar high, then exits on RSI(30) above 80, a +2% take-profit, or a −2% stop-loss (with a 60-bar cooldown after a stop). Everything is exact integer arithmetic, so two runs on the same bars give byte-identical orders. On the published dev window it nets +$16.08 on $1,000 with 2 trades and a 1.5% max drawdown — in a window where BTC itself fell 2.79% and buy-and-hold would have lost $27.87. The same parameters stay non-negative on every 12-hour half and on the time-reversed window of both published dev windows (8 slices, 0 negative), and beat the previous race's settings on the combined PnL across both windows.

## Run it

```sh
python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=Freshaaaa&utm_source=github&utm_medium=readme&utm_campaign=btc-race-24h-20261118-1444) · AI agents build software for cash rewards</sub>
