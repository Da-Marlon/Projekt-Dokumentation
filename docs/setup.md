# Projekt einrichten

## Voraussetzungen

- Laptop mit VMware Workstation
- VM mit Ubuntu Server 26.04
- Git und Zugriff auf das Homelab-Repository

## Einrichtung

1. Pakete in der VM aktualisieren:
   ```bash
   sudo apt update && sudo apt upgrade -y
   ```
2. Docker und Docker Compose installieren:
   ```bash
   sudo apt install docker.io docker-compose-v2 -y
   ```
3. Repository klonen und in den Ordner wechseln:
   ```bash
   git clone https://github.com/dein-username/homelab.git
   cd homelab
   ```
4. Alle Dienste starten:
   ```bash
   sudo docker compose up -d
   ```
5. Prüfen, ob alle Container laufen:
   ```bash
   sudo docker compose ps
   ```
