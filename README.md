# Awesome-Streaming-ETL-Data-Ingestion

# Top Streaming ETL & Data Ingestion Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Real-Time Pipelines, Change Data Capture & Self-Hosted Data Integration*  
**Last updated: October 2026**

This repository tracks notable **commercial streaming ETL platforms** and **open-source projects** that ingest, transform, and load data in real time from databases, APIs, event streams, and applications into warehouses, lakes, and analytics platforms.

**Examples** include Amazon Kinesis Firehose, Confluent Cloud, Google Cloud Dataflow, Databricks Auto Loader, Azure Event Hubs Capture, Striim, Redpanda Cloud, Hevo Data, Airbyte Cloud, and Fivetran (the category leaders).

**Open-source emphasis**: Streaming ETL is one of the strongest open-source domains. **Apache Kafka** and **Redpanda** anchor event streaming. **Airbyte** and **Meltano** lead ELT, while **Debezium** dominates CDC. **Apache Flink** and **Kafka Connect** handle stream processing, and **Benthos/Redpanda Connect** enables code-free pipelines. **Vector** and **Apache NiFi** complete the ingestion layer. This section is heavily expanded.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Amazon Kinesis Firehose](https://aws.amazon.com/kinesis/data-firehose/)**  
  **AWS's fully managed streaming delivery service** — load data into S3, Redshift, OpenSearch, and Splunk without managing infrastructure. **Best for AWS-native streaming ingestion** .

- **[Confluent Cloud](https://www.confluent.io/confluent-cloud/)**  
  **The leading managed Kafka platform** — ksqlDB, Flink, connectors, and schema registry. **Best for enterprise event streaming** .

- **[Google Cloud Dataflow](https://cloud.google.com/dataflow)**  
  **Google's fully managed stream and batch processing** based on Apache Beam. **Best for unified batch/stream pipelines** .

- **[Databricks Auto Loader](https://www.databricks.com/)**  
  **Incremental data ingestion for lakehouses** — automatically detects and processes new files. **Best for Databricks lakehouse ingestion** .

- **[Azure Event Hubs Capture](https://azure.microsoft.com/en-us/products/event-hubs/)**  
  **Azure's event streaming with automatic capture** to Blob Storage and Azure Data Lake. **Best for Azure-native streaming** .

- **[Striim](https://www.striim.com/)**  
  **Real-time data integration and streaming analytics** — CDC, database replication, and cloud migration. **Best for enterprise real-time pipelines** .

- **[Redpanda Cloud](https://redpanda.com/)**  
  **Kafka-compatible streaming platform** with no Zookeeper or JVM. **Best for high-performance streaming** .

- **[Hevo Data](https://hevodata.com/)**  
  **No-code data pipeline platform** — 150+ connectors with automatic schema mapping. **Best for no-code ETL** .

- **[Airbyte Cloud](https://airbyte.com/)**  
  **Managed version of the leading open-source ELT platform** — 300+ connectors. **Best for open-source ELT with managed convenience** .

- **[Fivetran](https://www.fivetran.com/)**  
  **The leading managed ELT platform** — 500+ connectors with automatic schema evolution. **Best for enterprise ELT** .

## Open-Source GitHub Projects

### Event Streaming Platforms

- **[Apache Kafka](https://github.com/apache/kafka)**  
  **The de facto standard for event streaming**, Apache-2.0 licensed with **28,000+ GitHub stars** . **Distributed, fault-tolerant, high-throughput pub/sub messaging** . **Kafka Connect for source/sink connectors** and **Kafka Streams for stream processing** . **The foundation for most streaming ETL architectures** . **Best for enterprise event streaming at scale** .

- **[Redpanda](https://github.com/redpanda-data/redpanda)**  
  **Kafka-compatible streaming platform in C++**, BSL licensed (free for most uses) . **No Zookeeper, no JVM** — simpler operations . **10x faster than Kafka** in some benchmarks . **Best for teams wanting Kafka compatibility with better performance** .

- **[Apache Pulsar](https://github.com/apache/pulsar)**  
  **Distributed messaging and streaming platform**, Apache-2.0 licensed with **14,000+ GitHub stars** . **Multi-tenancy, geo-replication, and tiered storage** . **The main alternative to Kafka** . **Best for multi-tenant and geo-distributed streaming** .

- **[NATS](https://github.com/nats-io/nats-server)**  
  **Cloud-native messaging system**, Apache-2.0 licensed . **Lightweight, high-performance pub/sub** with JetStream for persistence . **Best for IoT and edge streaming** .

### ELT & Data Integration

- **[Airbyte](https://github.com/airbytehq/airbyte)**  
  **The leading open-source ELT platform**, MIT licensed with **16,000+ GitHub stars** . **300+ connectors for databases, APIs, and SaaS applications** . **Self-hosted or cloud** — full data control . **The de facto open-source Fivetran alternative** . **Best for open-source ELT at scale** .

- **[Meltano](https://github.com/meltano/meltano)**  
  **Open-source ELT platform built on Singer**, MIT licensed . **500+ taps and targets** — extract, load, and transform . **Best for Singer-based ELT pipelines** .

- **[Singer](https://github.com/singer-io)**  
  **The original open-source ELT specification** — taps (extract) and targets (load) . **The foundation for Meltano and other ELT tools** . **Best for understanding ELT architecture** .

- **[Apache SeaTunnel](https://github.com/apache/seatunnel)**  
  **High-performance data integration platform**, Apache-2.0 licensed . **Batch and stream processing with 100+ connectors** . **Best for large-scale data integration** .

- **[Apache NiFi](https://github.com/apache/nifi)**  
  **Open-source data flow automation**, Apache-2.0 licensed with **4,000+ GitHub stars** . **Visual programming for data routing, transformation, and ingestion** . **Best for data flow management** .

- **[Benthos (Redpanda Connect)](https://github.com/redpanda-data/connect)**  
  **Stream processing without code**, Apache-2.0 licensed with **8,000+ GitHub stars** . **Declarative YAML configuration for streaming ETL** . **Hundreds of connectors** — Kafka, MQTT, HTTP, databases . **Best for data engineers wanting stream pipelines without programming** .

- **[Vector](https://github.com/vectordotdev/vector)**  
  **High-performance observability data pipeline**, MPL-2.0 licensed with **18,000+ GitHub stars** . **Collect, transform, and route logs, metrics, and events** . **Rust-based for performance** . **Best for observability and log streaming** .

### Change Data Capture (CDC)

- **[Debezium](https://github.com/debezium/debezium)**  
  **The leading open-source CDC platform**, Apache-2.0 licensed with **10,000+ GitHub stars** . **Captures row-level changes from PostgreSQL, MySQL, MongoDB, Oracle, SQL Server, and more** . **Kafka Connect-based** — integrates with Kafka, Pulsar, and other sinks . **The de facto standard for CDC** . **Best for database replication and real-time sync** .

- **[Maxwell](https://github.com/zendesk/maxwell)**  
  **MySQL CDC to Kafka**, open-source . **Lightweight alternative to Debezium** . **Best for MySQL-only CDC** .

- **[Canal](https://github.com/alibaba/canal)**  
  **Alibaba's MySQL binlog incremental subscription**, Apache-2.0 licensed . **Best for MySQL CDC in Asia** .

- **[PGDeltaStream](https://github.com/beOweb/pgdelta)**  
  **PostgreSQL logical replication for streaming**, open-source . **Best for PostgreSQL CDC** .

### Stream Processing

- **[Apache Flink](https://github.com/apache/flink)**  
  **The de facto standard for stateful stream processing**, Apache-2.0 licensed with **24,000+ GitHub stars** . **Exactly-once semantics, event-time processing, and savepoints** . **The engine behind Alibaba's Singles' Day** . **Best for mission-critical stream processing** .

- **[Apache Spark Structured Streaming](https://github.com/apache/spark)**  
  **Unified batch and stream processing**, Apache-2.0 licensed . **Micro-batch with exactly-once semantics** . **Best for teams already using Spark** .

- **[Kafka Streams](https://github.com/apache/kafka)**  
  **Stream processing library for Kafka**, Apache-2.0 licensed . **No separate cluster** — runs in your application . **Best for Kafka-native stream processing** .

- **[ksqlDB](https://github.com/confluentinc/ksql)**  
  **Streaming SQL for Kafka**, Confluent Community License . **SQL interface for Kafka Streams** . **Best for SQL-proficient teams** .

- **[Apache Beam](https://github.com/apache/beam)**  
  **Unified programming model for batch and stream**, Apache-2.0 licensed . **Portable across Flink, Spark, Dataflow, and Samza** . **Best for portable pipelines** .

### Additional Strong Open-Source Options

- **Apache Flume** — Log aggregation (largely superseded) .
- **Logstash** — Data collection and transformation .
- **Fluentd** — Unified logging layer .
- **Fluent Bit** — Lightweight log processor .
- **Apache Sqoop** — Hadoop data transfer (retired) .
- **Embulk** — Pluggable bulk data loader .
- **dlt** — Python library for data loading .
- **dbt** — SQL-based transformation (not ingestion but complementary) .
- **Apache Airflow** — Workflow orchestration .
- **Dagster** — Data orchestration .
- **Prefect** — Modern workflow orchestration .

**Frameworks for building custom streaming ETL solutions**: Combine **Apache Kafka** or **Redpanda** for event streaming . Use **Airbyte** for ELT with 300+ connectors . Deploy **Debezium** for CDC from databases . Choose **Apache Flink** for stateful stream processing . Integrate **Benthos** or **Vector** for code-free pipelines and observability data . Note that true enterprise streaming ETL with managed infrastructure, global scale, and vendor-supported SLAs (Confluent Cloud, Fivetran, Striim) remains primarily commercial territory; open-source stacks provide strong event streaming, ELT, CDC, and stream processing foundations that require integration for complete data pipelines.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Streaming ETL platforms handle sensitive business data in motion. Self-hosted solutions require proper security hardening, access controls, and compliance with data privacy regulations.
- **License considerations**: Redpanda uses BSL (free for most uses but not OSI), ksqlDB uses Confluent Community License, and some CDC tools have specific licensing. Verify licensing against your use case before committing .
- **Open-source streaming ETL requires operational expertise** — Kafka clusters, Flink jobs, and CDC connectors require monitoring, tuning, and maintenance. Managed platforms shift this responsibility to the vendor.
- **Data quality and schema evolution are critical** — streaming pipelines must handle schema changes, late data, and exactly-once semantics. Test thoroughly before production .
- The open-source ecosystem provides strong event streaming, ELT, CDC, and stream processing foundations, but **managed infrastructure, global scale, and vendor-supported SLAs** remain primarily commercial offerings.

---

**Made for data engineers, platform teams, and organizations seeking data pipeline sovereignty.**  
Let's make streaming ETL and data ingestion more open, transparent, and reliable.
