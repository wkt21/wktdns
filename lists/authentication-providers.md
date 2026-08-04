# Authentication Providers

Domains related to identity and authentication that are commonly needed for login flows.

## Covered in Allowlists
- login.microsoftonline.com (Microsoft)
- gateway.icloud.com / api.apple.com (Apple)
- nextdns.io family (NextDNS management)

## Notes
When deploying aggressive denylists, always verify that your primary authentication providers remain reachable. Add additional IdP domains (Okta, Auth0, Google Workspace if needed, etc.) to the allowlist as required by your environment.
