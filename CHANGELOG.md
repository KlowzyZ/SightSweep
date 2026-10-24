# Changelog

All notable public SightSweep changes are documented here.

## [2.0.0] - 2026-10-25

- Broader layered IPv4 discovery and evidence enrichment, selected-interface handling, Quick/Thorough modes, exact ranges and redacted diagnostics.
- Compact results-focused workspace, virtualized/resizable columns, optional evidence pane, improved Settings/About and EN/TR/AR support.
- Saved networks, history/comparisons, local exports and confirmed cross-scan identities with revision-protected labels/notes and conservative ambiguity handling.
- Branded per-user Inno Setup installer, optional desktop shortcut, running-instance guard, in-place updates and uninstall that retains data; portable ZIP remains available.
- New profiles receive background daily Stable checks; explicit disabled choices remain unchanged. No scan data/telemetry is sent and updates never install automatically.
- Owner-tested scanning/interface; focused release gates cover updates/UI, per-user installer lifecycle/data retention and portable startup. No exhaustive device/routing/OS compatibility claim. Previous releases/assets are preserved.

## [1.0.0] - 2026-08-25

### Added

- Fast progressive IPv4 discovery using ARP, ICMP, bounded TCP probes, reverse DNS, and ONVIF WS-Discovery.
- Evidence-based device classifications that preserve unknown devices by IP.
- Specialized IP camera, NVR, DVR, ONVIF, and RTSP evidence.
- Scan cancellation, rescan, search, filters, device details, projects, local history, comparison, and CSV/JSON exports.
- English, Turkish, and Arabic user interfaces with Arabic right-to-left layout.
- Anonymous stable update checking with a default-enabled preference and 24-hour automatic throttle.
- Self-contained portable Windows x64 release with SHA-256 checksums and complete legal notices.

### Security and privacy

- No telemetry, advertising, cloud upload, credential guessing, exploitation, or Internet-wide scanning.
- Secure bounded ONVIF XML parsing with DTD and external entity processing disabled.
- Release links restricted to the expected HTTPS GitHub repository.

[1.0.0]: https://github.com/KlowzyZ/SightSweep/releases/tag/v1.0.0
