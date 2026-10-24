# Getting Started

## Requirements

- Windows 11 x64 is the primary tested platform.
- A local IPv4 network you own or are explicitly authorized to administer.
- No separate .NET installation, administrator privilege, Nmap, Npcap, or packet driver is required for a normal scan.

## Verify the download

Download `SHA256SUMS.txt` beside the executable, then run:

```powershell
Get-FileHash .\SightSweep-v2.0.0-win-x64.exe -Algorithm SHA256
```

Compare the resulting hash with the matching line in `SHA256SUMS.txt`.

The EXE is the per-user installer; close running SightSweep instances before installing/upgrading. It creates a Start Menu shortcut and offers an optional desktop shortcut. For portable use, extract the entire ZIP and run SightSweep.exe. Both options bundle .NET and are unsigned. Installation/uninstallation retains user data. Back up important data before upgrading; Preview profiles remain separate from Stable.

## Run a scan

1. Start SightSweep.
2. Review the compact network summary. Use its gear to open Network & workspace in Settings and confirm the intended adapter/source. Physical-interface/default-route metadata guides automatic recommendations; manual VPN/virtual sources remain available.
3. Confirm the authorized CIDR or exact start/end range, capped at 4,096 hosts. Automatic range follows the actual subnet; manual ranges remain explicit. Save settings to retain edits after restart, then use Back to scan. Network changes never start a scan automatically.
4. Select Quick or Thorough and press Start scan. Stop drains pending work before a rescan. Search/filter/sort results and resize table columns as needed.
5. Select a result to review reachability, service and classification evidence. Close or resize the evidence pane when needed.

Unknown devices remain in the table by IP. A missing classification is not treated as a missing device.

## Projects, history, and exports

Create or select a project before scanning to retain that session locally. The Reports page compares a selected session with its previous scan and exports credential-free CSV or JSON inventory data.

Cross-scan label/note links require confirmation; IP alone does not establish device identity. Duplicate, missing or randomized identifiers can prevent safe linkage. Stable retains `%LOCALAPPDATA%\SightSweep`; no Preview data is merged automatically. Avoid editing newer shared annotations with older builds.

## Updates

New profiles enable background Stable checks, throttled to approximately once every 24 hours. Explicit saved disabled choices remain disabled. Open Settings for manual checks or opt-out. The availability notice opens the public release page only after a user action; installation is never automatic. No scan data, credentials, telemetry or analytics are transmitted.

Coverage varies with devices, firewalls, VLANs, routes and isolation. The owner has tested their setup; exhaustive hardware, routing, physical DPI/accessibility and enterprise installation acceptance is not claimed. Inspect device exports for network identifiers before sharing.
