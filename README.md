# SnipEX Releases

This public repository is the official SnipEX binary-distribution, update-feed, checksum, and release-notes channel. Application source, synchronized snippets, account records, sessions, and Railway volume data are not published here.

## Current stable release

SnipEX Version 2.2.13 Stable is the current Windows employee-testing build. Use [SnipEx-2.2.13-win-x64-Setup.exe](https://github.com/PeterDenali/SnipEX-Releases/releases/download/v2.2.13/SnipEx-2.2.13-win-x64-Setup.exe) for a normal per-user installation. The `.msi` is provided for managed deployment, and the `.zip` is the portable testing package. Each package has a matching SHA-256 checksum file. Version 2.2.13 improves code organization and Windows update-feed reliability while preserving the existing interface and functionality, including the expansion, clipboard-safety, and snippet-selection fixes from 2.2.12.

The macOS 2.2.0 compatibility images remain available in the earlier Version 2.2.7 release while a newer Mac build awaits an approved macOS build/signing environment. They are clearly marked as legacy and are not advertised to the Windows automatic updater.

SnipEX reads the latest public GitHub Release directly. Older installed clients use the small compatibility manifests in this repository; both the root and Windows x64 manifests point to 2.2.13. Startup checks notify users and require **Update now** approval before downloading or installing. After approval, the in-client updater downloads the matching package, verifies its SHA-256 checksum, installs it without elevation, and restarts SnipEX without a browser handoff.

Railway remains responsible only for authorization and synchronized personal/Organization snippet data. It is not the installer host.

## Security

Only download SnipEX from the current release linked by this repository and verify the matching SHA-256 checksum. The employee-testing packages remain unsigned until an organization-approved code-signing process is available.
