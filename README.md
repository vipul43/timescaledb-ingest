# TimescaleDB ingest
A rust tool to ingest data into timescale db from various sources.

## Supported sources

* [ ] [Victoriametrics](https://victoriametrics.com)
* [ ] [Prometheus](https://prometheus.io)
* [ ] [InfluxDB](https://www.influxdata.com)
* [ ] [OpenTSDB](https://opentsdb.net)
* [ ] [Thanos](https://thanos.io)

## Idea

* `timescaledb-parallel-copy` is highly efficient and the offical tool suggested
  by [TigerData](https://www.tigerdata.com/blog/how-to-migrate-your-data-to-timescale)
* This tool accepts data in csv format, so the core idea is to generate csv files
  from different formats like jsonl, openmetric, etc, in a highly efficient and parallel
  way.
* Finally packaging the tool `timescaledb-ingest` along with `timescaledb-parallel-copy`.
* Or better building the entire solution from scratch taking full advantage of rust
  multi-thread. Hope I don't have to get to this!
  
## Technologies

* [Rust](https://www.rust-lang.org/)
    * [sqlx](https://github.com/launchbadge/sqlx)
* [timescaledb-parallel-copy](https://github.com/timescale/timescaledb-parallel-copy)

## Conventions

* [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)
* [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) 
* [Semantic Versioning](https://semver.org/spec/v2.0.0.html)
