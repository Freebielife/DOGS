# Dogs Observatory

## О проекте / токене

DOGS — токен в сети TON. В официальном канале проект описывает его как мем-токен сообщества Telegram, вдохновлённый персонажем Spotty Павла Дурова.

Краткое описание по указанным первичным источникам.

Источники (проверены 2026-11-23):

- <https://tonapi.io/v2/jettons/EQCvxJy4eG8hyHBFsZ7eePxrRsUQSFE_jpptRAYBmcG_DOGS>
- <https://dogs.dev/links>
- <https://t.me/dogs/2>

Generated from https://github.com/Freebielife/TON-Observatory-Template.

Run python3 -m scripts.refresh_observatory; python3 build.py; python3 verify.py.
Publish index.html in TON Sites only after independent on-chain verification.
The bundled snapshot contains collected on-chain data. Section freshness and incomplete history are shown in the interface.
Only native TON swap pairs supported. Locks, staking and custom project NFT badges are configured through project.json and verified against TonAPI.
A fallback GitHub Actions schedule is configured for minute 7 and 37 of every UTC hour. GitHub scheduled jobs may be delayed. Live Cloudflare dispatch is not yet connected.

Foundation version: 1.3.0. Holders show 10, expandable to top 20.
`project.json` is the per-project specification. Contract/pool/precision changes require regenerating from the factory; do not reuse another token's snapshot.
Run `python3 build.py` for an atomic bundle and `build/report.json` size report.
No external fonts, scripts or images are needed to render the saved page. Fresh data checks and manual wallet lookups require network access.
Cloudflare dispatch registration and GitHub repository access remain separate deployment steps. No credentials go into HTML.

## Branding and data coverage

Hero: token metadata logo (`https://cdn.dogs.dev/dogs.png`). Section artwork: user-selected TONecoFlags #035. Channel verified through https://dogs.dev/links: https://t.me/dogs.

Direct DOGS/TON swaps are collected from two swap-verified pools (DeDust and STON.fi). Other quotes are outside the transaction feed coverage. The chart uses the configured primary pool and current total supply; historical coverage expands incrementally and is labelled partial until complete. Unconfigured lock/staking sources remain unavailable.

Template commit: `c618b19f51fcfa44264e753a6945419d63934992` (engine 1.3.0). Rendering uses embedded resources; live snapshots and wallet lookup use network requests.
