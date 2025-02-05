

</head>
<body>
    <div class="container">
        <h1>AdGuard Docker Stack</h1>
        <p>The <span class="highlight">ultimate</span> self-hosted DNS solution for <strong>privacy, speed, and reliability</strong>—featuring <strong>AdGuard</strong>, <strong>Unbound</strong>, <strong>Redis</strong>, <strong>PowerDNS</strong>, and <strong>DNSCrypt-Proxy</strong>. This stack provides <strong>ad-blocking, encryption, caching, failover, and customizable DNS resolution</strong> in a lightweight and efficient Docker setup.</p>
        
        <h2>🚀 Features & Benefits</h2>
        <ul>
            <li><strong>AdGuard</strong>: Blocks ads, trackers, and malware at the DNS level, improving privacy and security.</li>
            <li><strong>Docker Compose Stack</strong>: Enables quick and effortless deployment and recovery.</li>
            <li><strong>Unbound with Redis</strong>: Offloads DNS caching to RAM for ultra-fast lookups.</li>
            <li><strong>PowerDNS & DNSCrypt-Proxy</strong>: Provides encryption, redundancy, and failover to ensure uninterrupted DNS resolution.</li>
            <li><strong>Easy Setup</strong>: Simply point your router’s DNS to the AdGuard instance—no extra configuration needed.</li>
            <li><strong>Multi-System Deployment</strong>: Easily deploy across two or more systems for high availability and redundancy.</li>
            <li><strong>Optimized Configuration</strong>: AdGuard’s caching is disabled to let Redis and Unbound handle it efficiently.</li>
            <li><strong>RAM-Optimized Logging</strong>: Logs are stored in RAM to reduce disk writes (configurable via <code>docker-compose.yml</code>).</li>
        </ul>

        <h2>🛠️ Quick Deployment</h2>
        <p>This stack enables a <strong>private, fast, and resilient</strong> DNS infrastructure in minutes. <strong>Unbound</strong> acts as the primary resolver, with <strong>Redis</strong> handling caching, while <strong>PowerDNS</strong> and <strong>DNSCrypt-Proxy</strong> provide high-performance encrypted failover support. Additional upstreams can be configured directly within AdGuard.</p>

        <h2>🔗 Related Projects & Configuration</h2>
        <ul>
            <li><a href="https://github.com/saint-lascivious/unbound-config" target="_blank">saint-lascivious/unbound-config</a> – Optimized Unbound configuration for privacy and performance.</li>
            <li><a href="https://github.com/trinib/AdGuard-WireGuard-Unbound-DNScrypt" target="_blank">trinib/AdGuard-WireGuard-Unbound-DNScrypt</a> – A modular setup integrating AdGuard, WireGuard, Unbound, and DNSCrypt-Proxy.</li>
        </ul>

        <h2>📌 Learn More About the Components</h2>
        <ul>
            <li><a href="https://github.com/AdguardTeam/AdGuardHome" target="_blank">AdGuard Home</a></li>
            <li><a href="https://github.com/NLnetLabs/unbound" target="_blank">Unbound</a></li>
            <li><a href="https://github.com/redis/redis" target="_blank">Redis</a></li>
            <li><a href="https://github.com/PowerDNS/pdns" target="_blank">PowerDNS</a></li>
            <li><a href="https://github.com/DNSCrypt/dnscrypt-proxy" target="_blank">DNSCrypt-Proxy</a></li>
        </ul>
    </div>
</body>
</html>
