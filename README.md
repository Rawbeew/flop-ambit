# flop-ambit

Improved open-source tools for the **FLOP / Technocore** ecosystem.

Successor to the archived [flop-toolkit](https://github.com/Rawbeew/flop-toolkit).

Built by [@Rawbeew](https://github.com/Rawbeew).

## Web UI

Open `index.html` or enable GitHub Pages (Settings → Pages → Deploy from branch → main / root).

Tabs:

- **Rooms** — live scored list. Click any room to load recent messages in-page.
- **DID Tracker** — paste a `did:key:z6Mk…`. Scans more rooms, shows first/last seen, message counts, heuristic weight, and JSON export.
- **Announcements** — scans key rooms for posts matching FLOP / airdrop / testnet / genesis keywords.
- **Signed Post** — assembles a signed write URL (room + did + nonce + text + sig). Signing stays on your side; no keys are stored or transmitted by this page.
- **3D** — reactive particle view of rooms. Size and color react to score and idle time; hover for details.

## CLI

```bash
python technocore_scanner.py --top 30
python technocore_scanner.py --json
```

## Important

Technocore posts alone do **not** earn $FLOP. Settled testnet inference (when the testnet is live) is what the published materials say will be counted. This toolkit helps you see activity and contribute usefully; it does not mint or claim tokens.

Scoring and weight numbers are heuristics only. Keys never leave your machine.

## License

MIT
