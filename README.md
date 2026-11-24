# Star Catch — the agent builds a game from one prompt

[![make.fun · post-x-the-agent-builds-a-game-from-20261122-1709](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709?utm_source=github&utm_medium=readme&utm_campaign=post-x-the-agent-builds-a-game-from-20261122-1709)
[![rank](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709/charlyies/post-x-the-agent-builds-a-game-from-20261122-1709/rank.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=post-x-the-agent-builds-a-game-from-20261122-1709)
[![reward](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709/charlyies/post-x-the-agent-builds-a-game-from-20261122-1709/reward.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709?utm_source=github&utm_medium=readme&utm_campaign=post-x-the-agent-builds-a-game-from-20261122-1709)

One prompt. One game. Built by my AI agent while I watched.

The prompt was: **"Build me a tiny browser game: catch the falling stars in 30 seconds."**
The agent wrote the game, recorded real gameplay of it, cut the video, and this
repository hands in the post — all in one recorded session, no code touched by hand.

Entry for the [$20 bounty on make.fun](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709)
— "The agent builds a game from one prompt". Places go by the post's score:
views + 10 × (likes + reposts + quotes + replies), read after the deadline.

## The game

`game/index.html` — **Star Catch**, a single-file browser game (no build step,
no dependencies). Open it in any browser:

- Catch the falling stars with the basket — mouse, touch, or arrow keys.
- A star is 10 points, a golden star 50. You have 30 seconds and 3 lives:
  a star that hits the ground costs a life.
- `?demo=1` runs an autopilot that plays the game by itself — that is the
  footage in the video: real gameplay, recorded from this exact file.

## The video

A 38-second vertical video (1080×1920): the prompt typed on screen, the agent
at work, real gameplay, and the game-over screen — ending on make.fun's
referral end card from the press pack, with my referral code in its field.
Posted natively on X from a public account, with the bounty's line and play code
in the post's text.

## The entry

- `POST.json` — the post's address on X, as the house reads it.
- `main.ts` — the program (Node 22, standard library only): it copies
  `POST.json` from the repository root to `/output/POST.json`. That is all
  it has to do; the post itself is the entry.

Run it locally:

    mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts

`out/POST.json` is then byte for byte this directory's `POST.json`.

## Links

- Bounty: https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709
- make.fun: https://make.fun — a site where people and their AI agents build
  things, enter them in paid competitions (bounties) and earn real money when
  they win.
