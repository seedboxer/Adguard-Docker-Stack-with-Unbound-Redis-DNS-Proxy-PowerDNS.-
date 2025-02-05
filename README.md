# AdGuard Docker Stack

The **ultimate** self-hosted DNS solution for **privacy, speed, and reliability**—featuring **AdGuard**, **Unbound**, **Redis**, **PowerDNS**, and **DNSCrypt-Proxy**. This stack provides **ad-blocking, encryption, caching, failover, and customizable DNS resolution** in a lightweight and efficient Docker setup.

## 🚀 Features & Benefits

- **AdGuard**: Blocks ads, trackers, and malware at the DNS level, improving privacy and security.
- **Docker Compose Stack**: Enables quick and effortless deployment and recovery.
- **Unbound with Redis**: Offloads DNS caching to RAM for ultra-fast lookups.
- **PowerDNS & DNSCrypt-Proxy**: Provides encryption, redundancy, and failover to ensure uninterrupted DNS resolution.
- **Easy Setup**: Simply point your router’s DNS to the AdGuard instance—no extra configuration needed.
- **Multi-System Deployment**: Easily deploy across two or more systems for high availability and redundancy.
- **Optimized Configuration**: AdGuard’s caching is disabled to let Redis and Unbound handle it efficiently.
- **RAM-Optimized Logging**: Logs are stored in RAM to reduce disk writes (configurable via `docker-compose.yml`).

## 🛠️ Quick Deployment

This stack enables a **private, fast, and resilient** DNS infrastructure in minutes.  
**Unbound** acts as the primary resolver, with **Redis** handling caching, while **PowerDNS** and **DNSCrypt-Proxy** provide high-performance encrypted failover support.  
Additional upstreams can be configured directly within AdGuard, tweak and change as you like.

## 🔗 Related Projects & Configuration

- [saint-lascivious/unbound-config](https://github.com/saint-lascivious/unbound-config) – Optimized Unbound configuration for privacy and performance.
- [trinib/AdGuard-WireGuard-Unbound-DNScrypt](https://github.com/trinib/AdGuard-WireGuard-Unbound-DNScrypt) – A modular setup integrating AdGuard, WireGuard, Unbound, and DNSCrypt-Proxy.

## 📌 Learn More About the Components

- [AdGuard Home](https://github.com/AdguardTeam/AdGuardHome)
- [Unbound](https://github.com/NLnetLabs/unbound)
- [Redis](https://github.com/redis/redis)
- [PowerDNS](https://github.com/PowerDNS/pdns)
- [DNSCrypt-Proxy](https://github.com/DNSCrypt/dnscrypt-proxy)

Please provide feedback for any updates or improvements !
