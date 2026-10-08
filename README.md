## Aleh Barodziy — Data Engineer

I build data pipelines for financial and crypto market data: ingestion from REST APIs and WebSockets, transformations in Spark and SQL, storage in PostgreSQL, ClickHouse and object storage, and the data marts and dashboards that analysts and traders use.

I also work on the trading side, so I know what market data means, where it breaks (gaps, late events, mismatched timestamps between sources) and what the people consuming it need.

Madeira, Portugal · open to remote Data Engineer roles

### Stack

**Languages**<br/>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" /> <img src="https://img.shields.io/badge/SQL-336791?style=flat-square&logo=postgresql&logoColor=white" alt="SQL" />

**Orchestration & processing**<br/>
<img src="https://img.shields.io/badge/Apache_Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white" alt="Apache Airflow" /> <img src="https://img.shields.io/badge/Apache_Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white" alt="Apache Spark" /> <img src="https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white" alt="dbt" />

**Storage & warehouses**<br/>
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL" /> <img src="https://img.shields.io/badge/ClickHouse-151515?style=flat-square&logo=clickhouse&logoColor=white" alt="ClickHouse" /> <img src="https://img.shields.io/badge/Greenplum-1E9E7E?style=flat-square" alt="Greenplum" /> <img src="https://img.shields.io/badge/Amazon_S3-569A31?style=flat-square&logo=amazons3&logoColor=white" alt="Amazon S3" />

**Ingestion**<br/>
<img src="https://img.shields.io/badge/REST_APIs-6BA539?style=flat-square&logo=openapiinitiative&logoColor=white" alt="REST APIs" /> <img src="https://img.shields.io/badge/WebSockets-010101?style=flat-square&logo=socketdotio&logoColor=white" alt="WebSockets" />

**Infrastructure & monitoring**<br/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker" /> <img src="https://img.shields.io/badge/Linux-333333?style=flat-square&logo=linux&logoColor=white" alt="Linux" /> <img src="https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white" alt="Grafana" /> <img src="https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white" alt="Prometheus" /> <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" alt="Git" />

**Also worked with**<br/>
<img src="https://img.shields.io/badge/Trino-DD00A1?style=flat-square&logo=trino&logoColor=white" alt="Trino" /> <img src="https://img.shields.io/badge/Apache_Iceberg-2F6FB7?style=flat-square" alt="Apache Iceberg" /> <img src="https://img.shields.io/badge/Hadoop-66CCFF?style=flat-square&logo=apachehadoop&logoColor=white" alt="Hadoop" /> <img src="https://img.shields.io/badge/Google_Cloud_Storage-4285F4?style=flat-square&logo=googlecloud&logoColor=white" alt="Google Cloud Storage" /> <img src="https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white" alt="pandas" /> <img src="https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white" alt="NumPy" /> <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white" alt="scikit-learn" /> <img src="https://img.shields.io/badge/LLM_agents-555555?style=flat-square" alt="LLM agents" />

### Selected projects

<!-- Uncomment after the CoinGecko project is published -->
<!--
**[CoinGecko batch pipeline](https://github.com/cryptotyk/REPO_NAME)**  
Airflow-orchestrated batch pipeline: CoinGecko REST API → raw JSON in S3 → Spark transformations → ClickHouse tables for analytics.  
`Python` `Airflow` `Spark` `S3` `ClickHouse` `Docker`
-->

**[Polymarket market telemetry](https://github.com/cryptotyk/polymarket-market-telemetry)**  
Python service that samples Polymarket order books (CLOB REST API), Chainlink reference prices (Polymarket RTDS WebSocket) and Binance spot/mark prices and klines into PostgreSQL, storing source timestamps and request latency with every sample. A Grafana dashboard compares the prediction-market price with the underlying asset in 5-minute crypto markets. Architecture write-up; code is private.  
`Python` `PostgreSQL` `SQLAlchemy` `WebSockets` `Docker Compose` `Grafana`

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

### Courses & certificates

- Interactive SQL Simulator — Stepik, 2026 · [certificate](https://stepik.org/cert/3330759)
- "Python Generation": course for beginners — Stepik, 2026 · [certificate](https://stepik.org/cert/3304082)
- Data Scientist. ML. Beginner level — Skillbox, 2025
- Fundamentals of Statistics and Probability Theory — Skillbox, 2025
- Fundamentals of Mathematics for Data Science — Skillbox, 2025
- Data Scientist. Analytics. Beginner level — Skillbox, 2024
- Python for Data Science — Skillbox, 2023

### Contact

[LinkedIn](https://www.linkedin.com/in/aleh-barodziy/) · [cryptotyk@gmail.com](mailto:cryptotyk@gmail.com)
