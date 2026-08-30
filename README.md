# Factory Monitoring System

## Overview
A monitoring solution designed to monitor servers,
Windows machines and network devices.

## Architecture

[Architecture Diagram]
``
                    +----------------------+
                    |       Grafana        |
                    |    Visualization     |
                    +----------+-----------+
                               |
                               |
                    +----------v-----------+
                    |     Prometheus       |
                    |   Metrics Storage    |
                    +----+------+----------+
                         |      |
             +-----------+      +------------+
             |                              |
             v                              v
    +----------------+              +----------------+
    | Windows        |              | Linux          |
    | Exporter       |              | Node Exporter  |
    +----------------+              +----------------+
             |
             |
             v
    +----------------+
    | Windows Server |
    +----------------+
`
                         |
                         v
                 +---------------+
                 | SNMP Exporter |
                 +-------+-------+
                         |
                         v
                 +---------------+
                 | Network Device|
                 +---------------+

                 
## Technologies
- Prometheus
- Grafana
- Docker
- SNMP
- Windows Exporter
- Node Exporter

## Features
- Server monitoring
- Windows monitoring
- Network device monitoring
- CPU/RAM monitoring
- Disk monitoring
- Network traffic monitoring

## Deployment

docker compose up -d

## Screenshots

[Dashboard screenshots]

## What I Learned
...
