# Personal Home Lab & Self-Hosted Infrastructure

A collection of Dockerized services running 24/7 on a Raspberry Pi 4. This repository contains the Infrastructure as Code (IaC) configurations used to deploy and manage my personal home server.

## 🛠️ Tech Stack & Architecture
* **Hardware:** Raspberry Pi 4 (ARM64)
* **OS:** Linux (RaspberryPi OS, Debian based)
* **Containerization:** Docker & Docker Compose
* **Networking & Security:** Tailscale (WireGuard) for Zero-Trust remote access
* **Reverse Proxy / HTTPS:** Tailscale Serve

## 🚀 Hosted Services
* **Pi-hole:** Network-wide ad blocking and local DNS sinkhole for enhanced privacy.
* **Vaultwarden:** Self-hosted password manager backend (Bitwarden compatible).
* **Heimdall:** Application dashboard and central hub for all running services.
* **Dashdot:** Modern, lightweight server resource monitoring (CPU, RAM, Storage, Temps).
* **Javagotchi Web:** A personal project which is a web application built with Java Spring Boot (for more info: https://github.com/AndreasKanell/JavagotchiWeb ).


## 🔒 Security Posture
All services are strictly isolated from the public internet. Remote access is exclusively managed via Tailscale's encrypted mesh network, ensuring robust security without exposing any router ports.