## Aleh Barodziy — Data Engineer

I build data pipelines for financial and crypto market data: ingestion from REST APIs and WebSockets, transformations in Spark and SQL, storage in PostgreSQL, ClickHouse and object storage, and the data marts and dashboards that analysts and traders use.

I also work on the trading side, so I know what market data means, where it breaks (gaps, late events, mismatched timestamps between sources) and what the people consuming it need.

Madeira, Portugal · open to remote Data Engineer roles

### Stack

- **Languages:** Python, SQL
- **Orchestration & transformation:** Apache Airflow, Apache Spark, dbt
- **Storage:** PostgreSQL, ClickHouse, Greenplum, S3
- **Ingestion:** REST APIs, WebSockets
- **Infrastructure & monitoring:** Docker, Linux (cron, systemd), Prometheus, Grafana, Git
- **Also worked with:** Trino, Apache Iceberg, Hadoop, Google Cloud Storage, pandas, NumPy, scikit-learn, LLM agents

### Selected projects

<!-- Uncomment after the CoinGecko project is published -->
<!--
**[CoinGecko batch pipeline](https://github.com/cryptotyk/REPO_NAME)**  
Airflow-orchestrated batch pipeline: CoinGecko REST API → raw JSON in S3 → Spark transformations → ClickHouse tables for analytics.  
`Python` `Airflow` `Spark` `S3` `ClickHouse` `Docker`
-->

<!-- Uncomment after the telemetry part is published as a public repo -->
<!--
**[Polymarket market telemetry](https://github.com/cryptotyk/REPO_NAME)**  
Python service that samples Polymarket order books (CLOB REST API), Chainlink reference prices (Polymarket RTDS WebSocket) and Binance spot/mark prices and klines into PostgreSQL, storing source timestamps and request latency with every sample. A Grafana dashboard compares the prediction-market price with the underlying asset in 5-minute crypto markets.  
`Python` `PostgreSQL` `SQLAlchemy` `WebSockets` `Docker Compose` `Grafana`
-->

**[Solana DEX trades collector](https://github.com/cryptotyk/solana-dex-trades-collector)**  
Streaming collector for the Birdeye WebSocket API: discovers newly listed Solana tokens, subscribes to their swap transactions and writes each transaction as JSON to Google Cloud Storage, partitioned by token address. Built to run as a container on Google Cloud Run.  
`Python` `asyncio` `WebSockets` `Google Cloud Storage` `Cloud Run`

**[Exchange account monitoring dashboard](https://github.com/cryptotyk/Crypto-Monitor-Dashboard)**  
Grafana dashboard on PostgreSQL tables of exchange balances and trades: base/quote balances over time, trade notional, fees, trade count and trade history, filtered by exchange, subaccount and trading pair.  
`SQL` `PostgreSQL` `Grafana`

### Experience in brief

- **Data Engineer · Coinrate.pro · 2025–present** — Python ingestion from REST APIs and WebSockets into PostgreSQL and S3, Spark transformations and ClickHouse loads orchestrated with Airflow; 120+ PostgreSQL tables and 30+ dbt models behind analytical data marts and Grafana dashboards for client reporting; cron jobs and long-running services under systemd with retries, backfills, deduplication and a 5-minute data freshness target.
- **Data Analyst · GOTBIT Hedge Fund · 2024** — scheduled Python jobs loading trades, orders, positions and balances from exchange APIs into PostgreSQL and Greenplum; SQL datasets and Grafana dashboards for liquidity, exposure and execution quality.
- **Node operator / validator · 2021–2024** — 100+ blockchain nodes on Linux, monitored with Prometheus and Grafana.

Additional focus: trading and market microstructure, ML (scikit-learn) and LLM agents for data workflows.

### Contact

[LinkedIn](https://www.linkedin.com/in/aleh-barodziy/) · [cryptotyk@gmail.com](mailto:cryptotyk@gmail.com)
