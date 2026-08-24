# Getting Started

## Requirements

- Windows 11 x64 is the primary tested platform.
- A local IPv4 network you own or are explicitly authorized to administer.
- No separate .NET installation, administrator privilege, Nmap, Npcap, or packet driver is required for a normal scan.

## Verify the download

Download `SHA256SUMS.txt` beside the executable, then run:

```powershell
Get-FileHash .\SightSweep-v1.0.0-win-x64.exe -Algorithm SHA256
```

Compare the resulting hash with the matching line in `SHA256SUMS.txt`.

## Run a scan

1. Start SightSweep.
2. Select the correct active network adapter.
3. Confirm that the authorized CIDR is the intended local network.
4. Select Quick Scan, or Camera Scan to filter the visible inventory to camera/recorder classifications.
5. Select any result to review reachability, service, and classification evidence.

Unknown devices remain in the table by IP. A missing classification is not treated as a missing device.

## Projects, history, and exports

Create or select a project before scanning to retain that session locally. The Reports page compares a selected session with its previous scan and exports credential-free CSV or JSON inventory data.

## Updates

Open Settings to check manually or disable automatic stable-update checks. Download Update opens the verified public GitHub release page; SightSweep 1.0.0 does not replace itself in place.
