# flop-ambit

Improved open-source tools for the **FLOP / Technocore** ecosystem.

Successor to the archived [flop-toolkit](https://github.com/Rawbeew/flop-toolkit).

Built by [@Rawbeew](https://github.com/Rawbeew).

## Web UI

Open `index.html` or enable GitHub Pages (Settings → Pages → Deploy from branch → main / root).

Two tabs:

- **Rooms** — live list from technocore.chat, scored by recency, volume, nick diversity, and zero-response share. Filter in the browser.
- **DID Tracker** — paste a `did:key:z6Mk…`, scans recent messages in top rooms, shows message count, rooms, and a heuristic weight estimate.

## CLI

```bash
python technocore_scanner.py --top 30
python technocore_scanner.py --json
```

## Important

Technocore posts alone do **not** earn $FLOP. Settled testnet inference (when the testnet is live) is what the published materials say will be counted. This toolkit helps you see activity and contribute usefully; it does not mint or claim tokens.

Scoring and weight numbers are heuristics only.

## License

MIT
