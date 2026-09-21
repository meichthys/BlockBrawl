<div align="center">

<img src="./assets/banner.svg" alt="Block Brawl" width="100%">

[![License: MIT-0](https://img.shields.io/badge/License-MIT--0-3fd8c9)](./LICENSE)
[![Vanilla JavaScript](https://img.shields.io/badge/Vanilla-JavaScript-ffd166?logo=javascript&logoColor=121016)](./BlockBrawl.html)
[![Multiplayer WebRTC P2P](https://img.shields.io/badge/Multiplayer-WebRTC_P2P-ff6b4a)](#play)
[![Build Step: None](https://img.shields.io/badge/Build_Step-None-5be37a)](./BlockBrawl.html)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-b56cff)](#contributing)
[![GitHub stars](https://img.shields.io/github/stars/meichthys/BlockBrawl?style=social)](https://github.com/meichthys/BlockBrawl/stargazers)

### 🎮 [![Play Now](https://img.shields.io/badge/PLAY_NOW-ff6b4a?style=for-the-badge)](https://meichthys.github.io/BlockBrawl/BlockBrawl.html)

*One file. No install. No account. Send a link, drop blocks, brawl.*

</div>

---

## What is this

**Block Brawl** is a head-to-head Tetris-style battle. Clear lines to send garbage to
your opponent's board — clear two gold `?` blocks in the same line and you'll hand
them something worse. First one to bury the other loses.

The whole game — board, rules, and real-time networking — lives in a single
self-contained HTML file. There's no backend, no build step, and nothing to install.
Two people open the same link and they're playing.

## Features

- **Real peer-to-peer multiplayer.** Powered by [Trystero](https://github.com/dmotz/trystero) over WebRTC — match data flows directly between the two browsers, not through a server.
- **Shareable rooms.** Loading the page generates a private room link automatically. Send it to whoever you're playing and you're seated at the same table.
- **Local play too.** No connection? Share one keyboard, or split a touchscreen between two players.
- **11 surprise effects** that turn a good clear into a bad time for your opponent — see below.
- **Touch controls** with an on-screen pad and a "face each other" layout for playing on one device.
- Zero dependencies baked into the page beyond one CDN import for networking. No npm, no bundler, no server.

<details>
<summary><strong>Surprise catalogue</strong> (click to expand)</summary>

| Effect | What it does | Shake it |
|---|---|---|
| Blackout | Your stack goes dark — only the falling piece stays lit | Clear 1 line or wait 12s |
| Mirror | Left and right are swapped | Clear 2 lines or wait 15s |
| Upside Down | Board is flipped and mirrored | Clear 1 line or wait 12s |
| Overclock | Gravity triples | Place 8 pieces or wait 15s |
| Fog | Next/Hold previews and the ghost piece vanish | Clear 1 line or wait 15s |
| Zigzag Rations | Your next four pieces are all S and Z | Place those 4 pieces |
| Ice Rink | Left/right taps slide the piece all the way to the wall | Wait 15s |
| Weeds | A rubble block sprouts on your stack every 2s | Clear 2 lines or wait 16s |
| Lead Boots | Pieces lock the instant they land — no sliding, no tucking | Place 6 pieces or wait 15s |
| Hold Lock | Hold is disabled and whatever you were holding is gone | Wait 20s |
| Tremor | Every row lurches sideways, wrapping at the edges | Instant — dig yourself out |

</details>

## Play

### Online

**[▶ Play Block Brawl](https://meichthys.github.io/BlockBrawl/BlockBrawl.html)**

Loading the page hands you a link with a room code baked in — copy it from the panel
and send it to whoever you're playing. Opening that link seats them at the same
table automatically.

> The play link above requires GitHub Pages to be enabled for this repo
> (**Settings → Pages → Deploy from a branch → `main` / `/ (root)`**). It's a one-time,
> one-click setup if it isn't already on.

### Locally

No hosting required — it's one file:

```bash
git clone https://github.com/meichthys/BlockBrawl.git
cd BlockBrawl
open BlockBrawl.html   # or just double-click it
```

Two people can also each run their own local copy and still play each other — the
matchmaking works over the internet regardless of where the file itself came from.

## Controls

| Action | Player 1 | Player 2 |
|---|:---:|:---:|
| Move | `A` `D` | `←` `→` |
| Soft drop | `S` | `↓` |
| Rotate | `Q` `W` | `/` `↑` |
| Hold | `E` | `R Shift` |
| Hard drop | `Space` | `Enter` |

Touch users get an on-screen button pad automatically.

## Contributing

Issues and pull requests are welcome. Since it's a single HTML file, most changes
are as simple as editing `BlockBrawl.html` directly:

1. Fork the repo and create a branch for your change.
2. Open `BlockBrawl.html` in a browser to test — no build step needed.
3. Open a pull request describing what changed and why.

Please keep it a dependency-free, single-file page — that's the point of it.

## License

Block Brawl is licensed under [MIT-0](./LICENSE) (MIT No Attribution) — do
whatever you want with it, no credit required.

## Support

If you enjoy Block Brawl, consider supporting its development:

<noscript><a href="https://liberapay.com/meichthys/donate"><img alt="Donate using Liberapay" src="https://liberapay.com/assets/widgets/donate.svg"></a></noscript>
