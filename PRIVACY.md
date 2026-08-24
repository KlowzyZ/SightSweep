# Privacy

SightSweep is local-first.

- Scan results, discovered IP and MAC addresses, hostnames, projects, history, comparisons, and exports remain on the local computer.
- SightSweep has no telemetry, analytics, advertising, account, or cloud upload.
- Credentials are not requested or retained by version 1.0.0. ONVIF discovery is credential-free.
- Local application data is stored under the current Windows user's local application-data directory.

## Update checks

Automatic stable-update checks are enabled by default and can be disabled in Settings. SightSweep makes an anonymous HTTPS GET request to:

`https://api.github.com/repos/KlowzyZ/SightSweep/releases/latest`

The request contains standard HTTP and GitHub API headers plus the installed SightSweep version. It does not include scan results, projects, network identifiers, credentials, or analytics. Automatic attempts are limited to once per 24 hours. A manual check always requests fresh public metadata.

When an update exists, SightSweep opens only the verified `https://github.com/KlowzyZ/SightSweep` release page after the user selects Download Update.
