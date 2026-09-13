# ccxt-paper

> ccxt · paper · multi-venue

[![Python 3.11+](https://img.shields.io/badge/python-3.11+-3776AB)](https://python.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Build](https://img.shields.io/badge/build-passing-brightgreen)]()

CCXT-shaped paper trader — stub ticker, fee, equity print.

## Features

- Default venue binance / BTCUSDT
- Built-in paper strategy plus paper mode
- Risk manager with daily-loss kill switch
- OHLCV store and SHA-256 stub candles
- Backtester with fill + fee model
- Click CLI: backtest, paper, status, orders

## Prerequisites

- Python 3.11+
- Git

## Getting Started

```bash
git clone <repo-url>
cd ccxt-paper
python -m pip install -e .
python -m ccxtpaper --help
```

## CLI Usage

```bash
ccxtpaper backtest --bars 200
# Replay stub candles

ccxtpaper paper
# Start a paper session

ccxtpaper status
# Print engine state

ccxtpaper orders
# List simulated fills
```

## Project Structure

```
ccxtpaper/
  core/        engine + risk
  strategy/    grid / dca / ema hooks
  exchange/    stub order client
  data/        candles + backtest
  cli.py
tests/
```

## Configuration

See `ccxtpaper/config.py`.

| Setting | Default | Description |
|---------|---------|-------------|
| `exchange` | `binance` | Venue id |
| `symbol` | `BTCUSDT` | Default pair |
| `strategy` | `paper` | Active strategy |
| `mode` | `paper` | paper or backtest |

## Tests

```bash
python -m pytest -q
```

## Background

The default Python query when someone wants a paper CCXT bot.

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.


---

## Topics

![ccxt](https://img.shields.io/badge/ccxt-111827?style=flat-square) ![paper](https://img.shields.io/badge/paper-111827?style=flat-square) ![ccxt-paper](https://img.shields.io/badge/ccxt%20paper-111827?style=flat-square) ![trading-bot](https://img.shields.io/badge/trading%20bot-111827?style=flat-square) ![crypto-trading](https://img.shields.io/badge/crypto%20trading-111827?style=flat-square) ![binance](https://img.shields.io/badge/binance-111827?style=flat-square) ![defi](https://img.shields.io/badge/defi-111827?style=flat-square) ![algorithmic-trading](https://img.shields.io/badge/algorithmic%20trading-111827?style=flat-square)

`ccxt` `paper` `ccxt-paper` `trading-bot` `crypto-trading` `binance` `defi` `algorithmic-trading` `quantitative-finance` `open-source` `python`

Search: ccxt-paper · ccxt · paper · multi-venue · CCXT-shaped paper trader — stub ticker, fee, equity print.

---

<sub>CCXT-shaped paper trader — stub ticker, fee, equity print.</sub>
