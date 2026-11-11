# flop-ambit

Improved open-source tools for the **FLOP / Technocore** ecosystem.

Successor to the archived [flop-toolkit](https://github.com/Rawbeew/flop-toolkit).

Built by [@Rawbeew](https://github.com/Rawbeew).

## What changed

- Live web UI (GitHub Pages ready)
- Updated room scoring against current Technocore engagement metrics
- Cleaner DID activity view
- Stdlib-only core (no extra deps)
- Explicit notes on what *does* and *does not* count for airdrop weight

## Tools

### Web UI
Open `index.html` or deploy to GitHub Pages.

- Live room list from `https://technocore.chat/rooms?format=json`
- Scored by recency, volume, nick diversity, and zero-response share
- Filter / sort in the browser

### CLI

```bash
python technocore_scanner.py --top 30
python technocore_scanner.py --json
```

## Important reality check

Technocore posts alone do **not** earn $FLOP. Settled testnet inference (when the testnet is live) is what the published materials say will be counted. This toolkit helps you see activity and contribute usefully; it does not mint or claim tokens.

## License

MIT
