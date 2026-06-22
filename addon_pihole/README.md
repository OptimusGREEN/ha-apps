![Total installs](https://img.shields.io/endpoint?url=https://analytics.home-assistant.io/addons_badge/OptimusGREEN/ha-apps/og_pihole.json)

# Pi-hole Add-on

Network-wide DNS ad blocking powered by [Pi-hole](https://pi-hole.net/).

## About

Pi-hole acts as a DNS sinkhole that blocks ads and trackers at the network level for every device on your network — no per-device configuration required.

## Features

- Blocks ads and trackers at the DNS level for your entire network
- Web UI for managing block lists and viewing statistics
- Supports `amd64`, `aarch64`, and `armv7` architectures

## Installation

1. Add this repository to your Home Assistant instance (see the [main README](../README.md)).
2. In the Add-on Store, find **Pi-hole** and click **Install**.

## Configuration

| Option | Default | Description |
|--------|---------|-------------|
| `webpassword` | *(empty)* | Password for the Pi-hole web interface |
| `timezone` | `UTC` | Your local timezone (e.g. `Europe/London`) |
| `dns_listening_mode` | `all` | DNS listening mode (`all`, `single`, `bind`, or `none`) |
| `web_port` | `80` | HTTP port for the web UI |
| `web_https_port` | `443` | HTTPS port for the web UI |

## Usage

After installation, open the Pi-hole web interface at `http://<your-ha-ip>/admin`.

To use Pi-hole as your network DNS, point your router's DNS server to the IP address of your Home Assistant instance.
