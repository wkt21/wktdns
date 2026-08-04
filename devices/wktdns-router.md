# WKT-DNS Router Deployment Notes

## Overview
Deploy the WKT-DNS unified lists on a router running Pi-hole, AdGuard Home, or NextDNS CLI / linked configuration.

## Pi-hole / AdGuard Home
1. Add the domains from `config/nextdns-denylist.txt` (or the unified master list) as blocked domains / custom blocklist.
2. Add the domains from `config/nextdns-allowlist.txt` as whitelist / allowed domains.
3. Prefer exact domain matching or the format required by your software.
4. Restart DNS service after importing.

## NextDNS on Router
- Use the NextDNS linked configuration or CLI.
- Apply the denylist and allowlist files directly.
- Point the router’s DNS to NextDNS endpoints so all downstream devices inherit the policy.

## Best Practices
- Start with logging enabled.
- Verify that Apple and Microsoft core services remain functional on client devices.
- Document any additional local exceptions (printers, NAS, internal services).
- Consider a separate “guest” or “IoT” network with even stricter rules.

## Files to Use
- Primary: `config/unified-master-list.txt` or the platform-specific files under `config/`.
