# habibi-boost-socks4-1 - ProxRipper SOCKS4 FIRST 50k Booster

SOCKS4 proxy booster (FIRST 50k) from ProxRipper.

- **Source:** `https://raw.githubusercontent.com/Mohammedcha/ProxRipper/refs/heads/main/full_proxies/socks4.txt` - **FIRST 50k (0-50000)**
- **Pipeline:** Load persistent dead list -> fetch FIRST 50k -> dead-first filter -> validate via `httpbin.org/ip` via `socks4://` (100 concurrency) -> update dead list (never deleted) -> geolocate working via `ip-api.com/batch` -> save `data/live_proxies.json`, `country/<CC>/socks4.txt`
- **Schedule:** Every 1 hour + manual dispatch
