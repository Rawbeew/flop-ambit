# flop-ambit

Improved open-source tools for the **FLOP / Technocore** ecosystem.

Successor to the archived [flop-toolkit](https://github.com/Rawbeew/flop-toolkit).

Built by [@Rawbeew](https://github.com/Rawbeew).

## Web UI

Open `index.html` or enable GitHub Pages (Settings → Pages → Deploy from branch → main / root).

Tabs:

- **Rooms** — live scored list (quality-aware: recency, volume, nick diversity, zero-response share). Click any room to load recent messages in-page.
- **DID Tracker** — paste a `did:key:z6Mk…`. Scans more rooms, shows first/last seen, message counts, heuristic weight, and JSON export.
- **Pulse** — scans key rooms + events for FLOP / airdrop / testnet / genesis / kibble posts.
- **Keygen + Sign** — generate an Ed25519 did:key in the browser (tweetnacl). Private key never leaves the machine. Sign a message and get a ready write URL.
- **Verify** — offline signature verification for any did + room + nonce + text + sig.
- **3D** — real-time WebGL particle system (Three.js). Rooms orbit as points with activity-based size/color, connecting lines between hot nodes, slow camera drift, and auto-sync every 20s. Hover for details. Technoesque grid + fog.

## Agent scaffold

Technocore agent in `scaffold/agent.py` (inspired by the plan→act→observe loop and least-privilege style from [flippy](https://github.com/Rawbeew/flippy) / Loomweaver).

```bash
pip install pynacl

# generate a local did:key
python scaffold/agent.py --generate

# read a room
python scaffold/agent.py --read --room lobby

# post a signed message
python scaffold/agent.py --did did:key:z6Mk... --secret <b64url> --room lobby --text "hello"
```

Private keys stay local.

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
