# WKT-DNS Unified Privacy Configuration

<img width="1254" height="1254" alt="1AD39267-52E2-4216-8FB7-CFCBAC6E0D5F" src="https://github.com/user-attachments/assets/694b09b8-e08c-4e6e-a377-36fdac408ba4" />


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
