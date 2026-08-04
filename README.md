# WKT-DNS Unified Privacy Configuration

WKT-DNS is a hardened DNS privacy configuration designed for:
- NextDNS
- Safari Screen Time
- Firefox (uBlock Origin)
- Pi-hole / AdGuard Home

This repository provides:
- A maximum tracking denylist
- A safe allowlist for Apple, Microsoft, and core internet services
- Platform-specific filter formats
- Documentation for each domain category
- Device-specific notes (iPhone 13, WKT-DNS router)

## Quick Start

### NextDNS
Use:
- `config/nextdns-denylist.txt`
- `config/nextdns-allowlist.txt`

### Safari (iOS/macOS)
Use:
- `config/safari-denylist.txt`
- `config/safari-allowlist.txt`

### Firefox (uBlock Origin)
Use:
- `config/ublock-filters.txt`

### Unified Master List
Use:
- `config/unified-master-list.txt`

## Domain Categories
See `/lists/` for breakdowns:
- Google tracking
- YouTube telemetry
- Meta tracking
- TikTok tracking
- Apple core services
- Microsoft core services
- CDN infrastructure
- Authentication providers

## Devices
See `/devices/` for deployment notes:
- iPhone 13
- WKT-DNS router

## License
MIT License
