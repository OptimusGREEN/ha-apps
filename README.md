# OptiHAPPS
Home Assistant Add-ons by OptimusGREEN

## Installation

### One-click install
Click the button below to add this repository to your Home Assistant instance:

[![Open your Home Assistant instance and show the add add-on repository dialog with a specific repository URL pre-filled.](https://my.home-assistant.io/badges/supervisor_add_addon_repository.svg)](https://my.home-assistant.io/redirect/supervisor_add_addon_repository/?repository_url=https%3A%2F%2Fgithub.com%2FOptimusGREEN%2Fha-apps)

### Manual install
1. In Home Assistant, go to **Settings → Add-ons → Add-on Store**.
2. Click the **⋮** menu (top right) and select **Repositories**.
3. Paste the following URL and click **Add**:
   ```
   https://github.com/OptimusGREEN/ha-apps
   ```
4. Close the dialog. The add-ons from this repository will now appear in the store.
5. Find the add-on you want, click it, then click **Install**.

## Available Add-ons

### Pi-hole
Network-wide DNS ad blocking powered by [Pi-hole](https://pi-hole.net/).

**Features:**
- Blocks ads and trackers at the DNS level for your entire network
- Web UI for managing block lists and viewing statistics
- Supports `amd64`, `aarch64`, and `armv7` architectures

**Configuration options:**
| Option | Default | Description |
|---|---|---|
| `webpassword` | *(empty)* | Password for the Pi-hole web interface |
| `timezone` | `UTC` | Your local timezone (e.g. `Europe/London`) |
| `dns_listening_mode` | `all` | DNS listening mode (`all`, `single`, `bind`, or `none`) |
| `web_port` | `80` | HTTP port for the web UI |
| `web_https_port` | `443` | HTTPS port for the web UI |