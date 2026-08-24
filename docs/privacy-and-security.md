# Privacy and Security Details

SightSweep is designed for authorized local administration. It uses bounded asynchronous probes, treats responses as untrusted input, and avoids elevated packet-capture drivers.

## Local data

Projects, scan sessions, comparisons, and exports are stored for the current Windows user. They are never uploaded by SightSweep. Remove sensitive details before sharing screenshots, logs, or exports.

## Network behavior

- ARP and ICMP establish local reachability.
- A small bounded TCP set helps discover hosts that do not answer ICMP.
- Service and reverse-DNS enrichment run only for responsive hosts.
- Credential-free ONVIF WS-Discovery uses local multicast and secure bounded XML parsing.
- SightSweep does not guess passwords, exploit services, bypass access control, or scan the Internet.

## External connections

The only optional external request is the anonymous public GitHub stable-update check described in [PRIVACY.md](../PRIVACY.md). User-selected local device web links and the KLOWZY developer profile open in the default browser after strict URI construction or validation.
