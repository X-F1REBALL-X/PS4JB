# PS4JB

PS4 jailbreak / HEN host.

**Created by X-F1REBALL-X**

**Live:** https://x-f1reball-x.github.io/PS4JB/

## Firmwares

| Firmware | Chain | Status |
| --- | --- | --- |
| 13.02, 13.04, 13.50, 13.52 | Relapse | Working on this host |
| 7.00 – 11.02 | CSSFontFace + Lapse | Auto (untested on this host) |
| 11.03 – 12.02 | Slopkit | Auto (untested on this host) |
| 12.50 – 13.00 | Slopkit | Auto (untested on this host) |
| 6.00 – 6.69 | CSSFontFace + Lapse | Auto (untested on this host) |
| 6.70 – 6.72 | BadHoist | Entry page (limited) |
| 7.00 – 9.60 | PSFree + Lapse | `?chain=psfree` (untested) |

Router auto-picks the chain by firmware. Override with `?chain=cssfontface|psfree|slopkit|relapse|badhoist` or `?force=1`.

## Setup

1. Open the live link on the PS4 browser.
2. Wait for cache, then the jailbreak starts.
3. Wait for success.
4. If it fails, restart the console and try again.

## Notes

- After success with GoldHEN, turn off **Rest Mode support** in GoldHEN settings. Leaving it on can leave a white light on reboot or shutdown (common on many hosts/FW, not only 13.xx).
- If it still happens, also turn off FTP and BinLoader, or disconnect the internet before power off.
- White light = hold Power about 10 seconds to force off, then boot again.

## Layout

- `index.html` — FW detect, cache, Relapse jailbreak (one page)
- `jb.js` — Relapse 13.02–13.52
- `chains/cssfontface/` — CSSFontFace + Lapse/Netctrl
- `chains/psfree-lapse/` — PSFree + Lapse
- `chains/slopkit/` — Slopkit Lapse/Netctrl
- `chains/badhoist/` — assets only
- `third_party/` — mirrored patches / offsets / licenses

## License

See `LICENSE`, `NOTICE`, and `third_party/licenses/`.
