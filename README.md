# TucoFlyer-Grafana

Dashboards for Grafana, for analyzing Tuco Flyer time-series data.

The Bot-Controller has its own built-in UI for real-time data (250 Hz, low latency)
but we store historical data to an external InfluxDB instance for later analysis. This
data is sampled at a lower rate (currently 100 Hz) and delivered to the database in
batches.

I've been experimenting with both Chronograf and Grafana for analyzing this data,
and it looks like Grafana handles time navigation at this scale somewhat better, but
they both seem like good options.

This repository will be specifically about confiurations and other tools for using Grafana
with Tuco Flyer's InfluxDB database.
