# iPhone 13 – WKT-DNS Deployment Notes

## Recommended Configuration

1. **NextDNS** (preferred)
   - Install the NextDNS profile or use the NextDNS app.
   - Import `config/nextdns-denylist.txt` as a denylist.
   - Import `config/nextdns-allowlist.txt` as an allowlist.
   - Enable "Block ads & trackers" and any additional privacy features.

2. **Safari Content Blockers / Screen Time**
   - Use `config/safari-denylist.txt` and `config/safari-allowlist.txt` with compatible content-blocking profiles or Screen Time domain restrictions where supported.

3. **System DNS**
   - Point Wi-Fi and Cellular DNS to your NextDNS resolver endpoints.

## Known Considerations on iPhone 13
- Apple services (iCloud, App Store, Push Notifications, Maps) rely on the allowlisted domains.
- Aggressive blocking of Google/YouTube domains will break those apps and embedded players.
- Test critical apps after applying the lists.
- Keep NextDNS logs enabled initially for troubleshooting.

## Suggested NextDNS Settings
- Analytics: Off or minimal
- Logs: Temporary (for verification)
- Block lists: Custom only (use the provided files)
- Safe search / parental controls: Optional
