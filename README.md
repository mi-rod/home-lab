# mi-rod Home Lab Orchestration

A centralized repository for my home lab service configurations, utilizing Docker and modular service orchestration. This setup serves as the backbone for my personal media delivery, automation, and data monitoring experiments.

## 🚀 Projects & Stacks

### [Main Stack](./main/docker-compose.yml)
The core of my environment, handling media management, automation, and infrastructure:
* **Media Delivery:** Plex, Jellyfin, and Audiobookshelf.
* **Automation (The "Arrs"):** Full suite (Sonarr, Radarr, Prowlarr, Bazarr) for automated content management.
* **Downloads & Security:** Transmission-VPN routed through Surfshark and JDownloader.
* **Infrastructure:** Nginx Proxy Manager for SSL/DNS management and Portainer for container oversight.
* **Web Monitoring:** Change Detection integrated with Playwright-Chrome for automated data scraping and site monitoring.

### [Immich](./immich/docker-compose.yml)
High-performance photo management.
* **Optimization:** Configured with Intel QuickSync (VA-API) for hardware-accelerated transcoding and optimized job concurrency settings to handle large library imports efficiently.

### [Nextcloud](./nextcloud/docker-compose.yml)
Self-hosted productivity suite and private cloud storage, ensuring data sovereignty and seamless file synchronization across devices.

## 🛠️ Technical Specifications
* **Host OS:** Ubuntu Server.
* **Architecture:** Modular Docker Compose deployments with isolated bridge networks and host-mode networking where required (e.g., Home Assistant).
* **Storage & Data:** Utilizing `rclone` for cloud-to-local data migrations and `docker-gc` for automated resource cleanup and data hygiene.

## 📈 Data & Automation Focus
As a **Data Professional**, I utilize this lab to maintain a hands-on environment for:
* **Data Ingestion:** Automated scraping and change tracking.
* **Service Analytics:** Monitoring usage trends via Tautulli.
* **Systems Optimization:** Tuning hardware performance and resource allocation for containerized workloads.

---
*Maintained by [mi-rod](https://github.com/mi-rod)*
