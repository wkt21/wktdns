# Microsoft Core Services (Allowlist)

Essential Microsoft domains for authentication, Office 365, Windows Update, and related services.

## Authentication & Office
- login.microsoftonline.com
- office365.com
- outlook.office.com
- graph.microsoft.com
- windowsupdate.microsoft.com
- copilot.microsoft.com

## Telemetry (Selective)
- mobile.events.data.microsoft.com
- wps-picasso-pr.pubsub.azure.com

## Notes
Some Microsoft telemetry domains appear in both deny and allow contexts depending on configuration goals. Core auth and update domains are allowlisted to keep Windows and Microsoft 365 functional.
