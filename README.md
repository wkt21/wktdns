WKT-DNS Unified Privacy Configuration



WKT-DNS is a hardened DNS privacy configuration designed for:

• NextDNS
• Safari Screen Time
• Firefox (uBlock Origin)
• Pi-hole / AdGuard Home


This repository provides:

• A maximum tracking denylist
• A safe allowlist for Apple, Microsoft, and core internet services
• Platform-specific filter formats
• Documentation for each domain category
• Device-specific notes (iPhone 13, WKT-DNS router)


Quick Start

NextDNS

Use:

• config/nextdns-denylist.txt
• config/nextdns-allowlist.txt


Safari (iOS/macOS)

Use:

• config/safari-denylist.txt
• config/safari-allowlist.txt


Firefox (uBlock Origin)

Use:

• config/ublock-filters.txt


Unified Master List

Use:

• config/unified-master-list.txt


Domain Categories

See /lists/ for breakdowns:

• Google tracking
• YouTube telemetry
• Meta tracking
• TikTok tracking
• Apple core services
• Microsoft core services
• CDN infrastructure
• Authentication providers


Devices

See /devices/ for deployment notes:

• iPhone 13
• WKT-DNS router

Network Telemetry Report

This report provides a real‑world snapshot of DNS activity observed under the WKT‑DNS Unified Privacy Configuration. All queries were processed through encrypted DNS transports (DoH/DoT) with hardened blocklists and device‑specific filtering.

Summary

• Total Queries: 5,856
• Blocked Queries: 222
• Block Rate: 3.79%
• Encrypted DNS: 100% (no plaintext DNS leakage)


WKT‑DNS maintains a strict privacy posture while preserving full functionality for Apple, Microsoft, and core internet services.

---

Resolved Domains

Domains that resolved normally without being blocked:

• gateway.fe2.apple-dns.net — 55
• e6858.dsce9.akamaiedge.net — 54
• www.apple.com — 48
• mobile.events.data.microsoft.com — 41
• api.nextdns.io — 39
• copilot-copilot-msft-com.trafficmanager.net — 36


These represent standard OS, CDN, and service‑level traffic.

---

Blocked Domains

Domains blocked by security, privacy, or parental‑control filters:

• o4508134825000960.ingest.us.sentry.io — 27
• o1069899.ingest.us.sentry.io — 15
• sentry.io — 14
• incoming.telemetry.mozilla.org — 13
• mobile.events.data.microsoft.com — 12
• analytics.adjust.io — 9


All blocked domains fall under telemetry, analytics, or tracking categories.

---

Blocklist Activity

Top blocklists responsible for filtering:

• 1Hosts (Xtra) — 173
• HaGeZi Multi ULTIMATE — 151
• HaGeZi Multi PRO++ — 149
• hBlock — 140
• 1Hosts (Lite) — 135
• anti‑AD — 134


These lists collectively enforce maximum privacy while maintaining OS stability.

---

Devices

Devices generating DNS traffic:

• WKT‑DNS Router: 5,544 queries
• iPhone 13: 312 queries


The router handles the majority of traffic, with the iPhone producing normal background service queries.

---

IP Sources

IPv6 sources observed:

• 2601:540:c703:3320:4d23:78de:60db:79e6 — 5,824 (Comcast, Waynesburg, USA)
• 2607:fb91:8ed:893a:b478:13f1:50a:2bdf — 32 (T‑Mobile, Baltimore, USA)


These represent home network traffic and mobile device traffic.

---

Root Domain Distribution

Top root domains queried:

• *.nextdns.io — 4,198
• *.apple.com — 350
• *.com.akadns.net — 100
• *.aaplimg.com — 97
• *.apple-dns.net — 87
• *.sentry.io — 84


This distribution reflects normal OS behavior, CDN usage, and privacy‑filtered telemetry.

---

GAFAM Distribution

Percentage of queries associated with major tech ecosystems:

• Apple: 10.52%
• Microsoft: 2.72%
• Google: 2.7%
• Amazon: 0.19%
• Facebook: 0.05%
• Others: 83.82%


The high “Others” percentage indicates strong privacy filtering and minimal third‑party tracking.


License

MIT License
