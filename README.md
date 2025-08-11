# AdGuard Filters

This repository holds a lightweight allowlist for AdGuard Home, focused on avoiding false positives for banking, streaming, retail, productivity, and common CDN domains.

## Files
- `allowlist.txt` — Adblock syntax allowlist for AdGuard Home.

## How to use with AdGuard Home
1. Upload `allowlist.txt` to this repository's `main` branch.
2. Get the raw URL, which will look like:
   `https://raw.githubusercontent.com/SirOcelot/adguard-filters/main/allowlist.txt`
3. In AdGuard Home go to **Filters -> Allowlist -> Add allowlist -> Enter URL** and paste the raw link.
4. Save. AdGuard Home will fetch and keep it updated automatically.

## Local testing
You can test resolution after applying the allowlist:
```powershell
# Windows
nslookup netflix.com <adguard_ip>
```
```bash
# macOS/Linux
dig netflix.com @<adguard_ip>
```
