# ChirpStack MQTT Forwarder Installer for Multitech MTCAP AP3 Gateways

This script installs or updates the [ChirpStack MQTT Forwarder](https://www.chirpstack.io/) on Multitech MTCAP AP3 Gateways. It is designed to work specifically with these gateways and leverages SSH to remotely execute commands on the gateway.

## Features

- **Full Installation:** Downloads and installs the correct MQTT Forwarder package for Multitech MTCAP AP3 Gateways.
- **Configuration Update:** Updates the MQTT server settings in the forwarder's configuration file.
- **Service Management:** Starts or restarts the MQTT Forwarder using `monit` after configuration changes.
- **Interactive Setup:** Prompts for necessary credentials and settings to ensure proper installation and configuration.
- **Error Handling:** Checks for prerequisites such as `sshpass` and guides you on installing them if missing.

## Prerequisites

- **Multitech MTCAP AP3 Gateway:** This script is intended solely for use with these gateways.
- **SSH Access:** The gateway must be reachable via SSH.
- **sshpass:** The script uses `sshpass` for non-interactive SSH authentication.
  - On **Debian/Ubuntu**: Install with `sudo apt install sshpass`
  - On **macOS**: Install with Homebrew using `brew install sshpass`
- **Internet Connectivity:** Required for downloading the MQTT Forwarder package.

## Usage

1. **Download the Script:** Save the script to your local machine (e.g., `chirpstack_mqtt_forwarder.sh`). Or clone this repository
    ```bash
    git clone https://github.com/smn-s-arch/armatherm-mtcap.git
2. **Make the Script Executable:**  
   ```bash
   chmod +x chirpstack_mqtt_forwarder.sh

## License

This script is provided as-is, with no warranty. Use it at your own risk. Contributions and improvements are welcome.
