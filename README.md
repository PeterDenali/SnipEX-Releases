# SnipEX Releases

This public repository is the official SnipEX binary-distribution, update-feed, checksum, and release-notes channel. Application source, synchronized snippets, account records, sessions, and Railway volume data are not published here.

## Current stable release

SnipEX Version 2.2.14 Stable is the current Windows employee-testing build. Use [SnipEx-2.2.14-win-x64-Setup.exe](https://github.com/PeterDenali/SnipEX-Releases/releases/download/v2.2.14/SnipEx-2.2.14-win-x64-Setup.exe) for a normal per-user installation. The `.msi` is provided for managed deployment, and the `.zip` is the portable testing package. Each package has a matching SHA-256 checksum file. Version 2.2.14 fixes optional-section editing and validates complete templates before saving, importing, previewing, or expanding. Existing expansion, clipboard-safety, synchronization, sign-in, and snippet-selection behavior is retained.

The macOS 2.2.0 compatibility images remain available in the earlier Version 2.2.7 release while a newer Mac build awaits an approved macOS build/signing environment. They are clearly marked as legacy and are not advertised to the Windows automatic updater.

SnipEX reads the latest public GitHub Release directly. Older installed clients use the small compatibility manifests in this repository; the root and Windows manifests point to 2.2.14. Windows ARM64 uses the x64 compatibility package, not a native ARM64 build. Startup checks notify users and require **Update now** approval before downloading or installing. After approval, the in-client updater downloads the matching package, verifies its SHA-256 checksum, installs it without elevation, and restarts SnipEX without a browser handoff.

Railway remains responsible only for authorization and synchronized personal/Organization snippet data. It is not the installer host.

## Retained releases

The September 15, 2026 cleanup removed superseded Windows releases 2.2.8–2.2.10. The September 16 patch does not delete any further releases or install anything on employee devices:

| Release | Reason retained |
| --- | --- |
| 2.2.14 | Current Windows release and update target |
| 2.2.13 | Previous Windows release retained for controlled rollback |
| 2.2.12 | Earlier rollback package retained; not an update target |
| 2.2.11 | Previous Windows ARM64 x64-compatibility target retained; no longer referenced by current feeds |
| 2.2.7 | Hosts the macOS 2.2.0 legacy images referenced by the Mac manifests; its existing assets are preserved |

Do not remove a release while a compatibility manifest still references its assets. Retained older packages are not recommendations to downgrade. Release cleanup does not uninstall or alter already installed clients.

## Security

Only download SnipEX from the current release linked by this repository and verify the matching SHA-256 checksum. The employee-testing packages remain unsigned until an organization-approved code-signing process is available.
