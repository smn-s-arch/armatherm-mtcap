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

  
 # ChirpStack MQTT Forwarder Installer für Multitech MTCAP AP3 Gateways

Dieses Skript installiert oder aktualisiert den [ChirpStack MQTT Forwarder](https://www.chirpstack.io/) auf Multitech MTCAP AP3 Gateways. Es ist speziell für diese Gateways ausgelegt und nutzt SSH, um Befehle aus der Ferne auf dem Gateway auszuführen.

## Funktionen

- **Komplettinstallation:** Lädt das passende MQTT Forwarder-Paket für Multitech MTCAP AP3 Gateways herunter und installiert es.
- **Konfigurationsaktualisierung:** Aktualisiert die MQTT-Server-Einstellungen in der Konfigurationsdatei des Forwarders.
- **Dienstverwaltung:** Startet den MQTT Forwarder nach Konfigurationsänderungen über `monit` neu.
- **Interaktive Einrichtung:** Fordert zur Eingabe notwendiger Zugangsdaten und Einstellungen auf, um eine korrekte Installation und Konfiguration sicherzustellen.
- **Fehlerbehandlung:** Überprüft Voraussetzungen wie `sshpass` und gibt Hinweise zur Installation, falls diese fehlen.

## Voraussetzungen

- **Multitech MTCAP AP3 Gateway:** Dieses Skript ist ausschließlich für diese Gateways vorgesehen.
- **SSH-Zugang:** Das Gateway muss per SSH erreichbar sein.
- **sshpass:** Das Skript verwendet `sshpass` für eine nicht-interaktive SSH-Authentifizierung.
  - Unter **Debian/Ubuntu**: Installation mit `sudo apt install sshpass`
  - Unter **macOS**: Installation mit Homebrew über `brew install sshpass`
- **Internetverbindung:** Erforderlich zum Herunterladen des MQTT Forwarder-Pakets.

## Verwendung

1. **Skript herunterladen:** Lade das Skript auf deinen lokalen Rechner herunter (z. B. `chirpstack_mqtt_forwarder.sh`) oder klone dieses Repository:
    ```bash
    git clone https://github.com/smn-s-arch/armatherm-mtcap.git
    ```
2. **Skript ausführbar machen:**  
    ```bash
    chmod +x chirpstack_mqtt_forwarder.sh
    ```
