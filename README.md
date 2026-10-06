# Predict.fun Crypto Up/Down Market Data — Full Edition · Free Sample

[Predict.fun historical data](https://outcometick.com/predict-fun-data) for the crypto Up/Down markets, collected 24/7 by [OutcomeTick](https://outcometick.com). This repository hosts a **free sample** of the
full edition: one real, unmodified UTC day (2026-09-08), laid out exactly as the delivered archive, so code
written against the sample runs unchanged on the full data.

> **中文：** 本仓库是 [OutcomeTick](https://outcometick.com/zh) 采集的[Predict.fun 历史数据](https://outcometick.com/zh/predict-fun-data)（加密 Up/Down 市场）完整版的**免费样本**：一个真实、未经修改的
> UTC 日（2026-09-08），目录结构与正式交付的数据完全一致，针对样本写的代码可以原样用在正式数据上。

## Download / 下载

**[predict-fun-data-samples.tar.gz](https://github.com/outcometick/predict-fun-data-samples/releases/latest/download/predict-fun-data-samples.tar.gz)**

```bash
curl -L https://github.com/outcometick/predict-fun-data-samples/releases/latest/download/predict-fun-data-samples.tar.gz | tar xz
```

Per-file row counts and sha256: [`samples/manifest.json`](samples/manifest.json).
Field reference: [DATA_GUIDE.md](DATA_GUIDE.md) · 中文字段说明：[数据使用说明.md](数据使用说明.md)

## What the full edition contains / 完整版包含的数据

- **[Order book](https://outcometick.com/predict-fun-order-book-data) snapshots** — full depth on both sides, for 5-minute, 15-minute, hourly and daily markets
- **Markets** — opening price, closing price and settled outcome
- **Prices** — the Chainlink price the venue relays, per second
- **Klines** — OHLC built from that price stream
- Predict.fun order books are full snapshots: there is no incremental stream and no trade stream

> **中文：** 盘口快照（5 分钟 / 15 分钟 / 小时 / 日线）、市场信息（开盘价、收盘价、结算结果）、平台推送的 Chainlink 价格流、K 线；Predict.fun 盘口为全量快照，没有增量流与成交流。

## Files in this sample / 样本包含的文件

| path | rows |
|---|---|
| `data/predict-fun/prices/BTCUSDT/BTCUSDT-feed1-predict-prices-2026-09-08.csv.gz` | 82,342 |
| `data/predict-fun/orderbook/BTC-5M/BTC-5M-predict-orderbook-2026-09-08.jsonl.gz` | 478,603 |
| `data/predict-fun/markets/predict-markets-2026-09-08.jsonl.gz` | 1,245 |
| `data/predict-fun/klines/BTCUSDT/1m/BTCUSDT-feed1-1m-2026-09-08.csv.gz` | 1,440 |

## Learn more / 了解更多

- [OutcomeTick](https://outcometick.com) — prediction-market data for Polymarket and Predict.fun · [中文站](https://outcometick.com/zh)
- [Documentation](https://outcometick.com/docs) — quickstart and complete task examples · [中文文档](https://outcometick.com/zh/docs)
- [API reference](https://outcometick.com/docs/api) · [Data schemas](https://outcometick.com/docs/schemas) · [Settlement rules](https://outcometick.com/docs/settlement)
- [Settlement statistics for BTC](https://outcometick.com/data/predict-fun/btc) — per-asset data page
- [Backtest in the browser](https://outcometick.com/backtest) — run a strategy on the archive without downloading anything

The full data is delivered with an API key and downloaded by day, asset and interval.
正式数据通过 API key 交付，按天、按币种、按周期下载。

For research and backtesting only; not investment advice. / 仅供研究与回测，不构成投资建议。
