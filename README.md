# // AdGuard Docker Stack // Unbound & Redis/ PowerDNS / Dnscrypt-Proxy // (Sdns testing adding soon)

The **ultimate** self-hosted DNS solution for **privacy, speed, and reliability**—featuring **AdGuard**, **Unbound**, **Redis**, **PowerDNS**, and **DNSCrypt-Proxy**. This stack provides **ad-blocking, encryption, caching, failover, and customizable DNS resolution** in a lightweight and efficient Docker setup.

Use it as a boilerplate for your own setup or as is.

## 🌠 High Performance, Private, Secure and robust

0-10 msec DNS response times on requests. Even on low-power single-board hardware. The example below is Raspberry PI 3B with over 300K responses running on a very slow SD Card. (4 DNS servers)

![Total Time](https://raw.githubusercontent.com/seedboxer/Adguard-Docker-Stack-with-Unbound-Redis-DNS-Proxy-PowerDNS.-/refs/heads/main/totaltime.png)  
![DNS Response](https://raw.githubusercontent.com/seedboxer/Adguard-Docker-Stack-with-Unbound-Redis-DNS-Proxy-PowerDNS.-/refs/heads/main/dnsreponse.png)

## 🚀 Features & Benefits

- **AdGuard**: Blocks ads, trackers, and malware at the DNS level, improving privacy and security.
- **Docker Compose Stack**: Enables quick and effortless deployment and recovery. Always upto date containers.
- **Unbound with Redis**: Offloads DNS caching to RAM for ultra-fast lookups.
- **PowerDNS & DNSCrypt-Proxy**: Provides encryption, redundancy, and failover to ensure uninterrupted DNS resolution.
- **Easy Setup**: Simply point your router’s DNS to the AdGuard instance—no extra configuration needed.
- **Multi-System Deployment**: Easily deploy across two or more systems for high availability and redundancy.
- **Optimized Configuration**: AdGuard’s caching is disabled to let Redis and Unbound handle it efficiently.
- **RAM-Optimized Logging**: Logs are stored in RAM to reduce disk writes (configurable via `docker-compose.yml`).

## 🛠️ Quick Deployment

This stack enables a **private, fast, and resilient** DNS infrastructure in minutes.  
**Unbound** acts as the primary resolver, with **Redis** handling caching, while **PowerDNS** and **DNSCrypt-Proxy** provide high-performance encrypted failover support. (fixed IPs allocated within compose, add these to adguard as primary or failover, as your prefer)
Additional upstreams can be configured directly within AdGuard, tweak and change as you like.

## 🖥️ Easy Setup

- **Adguard**: Turn off all caching. Enter DNS upstream/ Bootstrap / Fallback and Private DNS server. 
- **Unbound**:  Edit Config/forward-records.conf and config/cachedb.conf making sure its up to date. ** Please note setting forward-records.conf can slow down unbound, only use in specific requirements or if your chosen forwarder is fast. You can pick internal or external servers. The file shown is for reference only.
- **PowerDNS**: Edit recursor.yml or if you prefer use the conf.
- **DNSCrypt-Proxy**: Edit /conf/dnscrypt-proxy.toml.

##  📓 Notes
  
- Use [Dns BenchMark](https://www.grc.com/dns/benchmark.htm) and/or [DnsPerf](https://www.dnsperf.com/) to edit unbound Adguard fallbacks or optimize your unbound forwarders / for speed user only local DNS as forwarders or no forwarders.
- Any other adjustments are purely optional.

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
