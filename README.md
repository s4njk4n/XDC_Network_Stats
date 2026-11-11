# XDC Network Stats

A fast, live stats page for the XDC Network, part of [XDC Outpost](https://xdcoutpost.xyz/).

**Live:** https://xdcoutpost.xyz/XDC_Network_Stats/

- **Chain head:** the best block with a live "last block" timer, average block time, TPS, gas price and epoch progress.
- **Tiles:** nodes in sync, masternodes, block propagation, latency, countries and price.
- **Chain activity:** charts of block time, transactions, gas and propagation, plus a feed of the latest blocks.
- **Map:** reporting nodes by location, with breakdowns by client version, Go version and OS.
- **Node table:** searchable and sortable, with pins for your own nodes (saved in your browser).
- **Networks:** Mainnet and the Apothem testnet.

## Data sources

- **Mainnet nodes, propagation and the 40-block charts:** a live websocket to the public XinFin stats server (`stats1.xinfin.network/primus`), the feed behind xinfin.network. If it can't be reached, the page falls back to its REST snapshot.
- **Apothem:** the newer stats backend's `/v2/snapshot`.
- **Latest blocks, masternodes and epochs:** public XDC RPC, with failover between endpoints.
- **Price:** CoinGecko.

## Deploy

Push `index.html`, `app.js`, `README.md` and `LICENSE`, then enable GitHub Pages from `main` / `(root)`. The page uses the shared Outpost styles, fonts and analytics from `/assets/` on xdcoutpost.xyz.

## Licence

MIT
