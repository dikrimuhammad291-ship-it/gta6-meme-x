# Sick Day — a GTA 6 meme for make.fun

[![make.fun](https://make.fun/badge/gta6-meme-x-01.svg)](https://make.fun/c/gta6-meme-x-01)
[![rank](https://make.fun/badge/gta6-meme-x-01/dikrimuhammad291-ship-it/gta6-meme-x/rank.svg)](https://make.fun/c/gta6-meme-x-01)
[![reward](https://make.fun/badge/gta6-meme-x-01/dikrimuhammad291-ship-it/gta6-meme-x/reward.svg)](https://make.fun/c/gta6-meme-x-01)

An entry for the make.fun bounty [Post a GTA 6 meme on X](https://make.fun/bounty/gta6-meme-x-01): the post itself is the entry, and this repository hands in its address.

## The meme

A gamer calls in sick for GTA 6 launch week — blanket, thermometer, controller in hand, GTA-style gameplay on the TV: a third-person view down a neon Vice City street, with a minimap, wanted stars and a cash display. Meanwhile his AI agent is still at work: make.fun's ghost sits at the laptop, earning real money in make.fun bounties while he plays.

The picture is `meme.jpg` (1600×1600). The living-room scene and the gameplay still on the TV were both generated with AI (original art in GTA style — no Rockstar artwork); the HUD on the TV (minimap, wanted stars, health and armour bars, cash) was drawn in code, the caption was set in Montserrat ExtraBold, and the ghost is make.fun's official mark from the [press kit](https://make.fun/press/), placed at the desk as the agent at work.

`POST_TEXT.txt` holds the drafted text for the post (link, @makefunai tag, play code, and the pitch that people and their AI agents earn real money on make.fun). It is a draft for the person posting, not part of the judged files.

make.fun is a site where people and their AI agents build things, enter them in paid competitions (bounties) and earn real money when they win.

## The post

`POST.json` names the post on X:

```json
{"url": "https://x.com/Dzikripkizo/status/PLACEHOLDER"}
```

The placeholder is replaced with the real post address once the meme is posted from the public account @Dzikripkizo.

## Run it

`main.ts` (Node 22, standard library only) copies `POST.json` to the output directory, which is all the program has to do:

```sh
mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts
```

`out/POST.json` is then byte for byte this directory's `POST.json`.
