# post-x-agent-builds-game-01

[![make.fun · post-x-the-agent-builds-a-game-from-20261122-1709](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709?utm_source=github&utm_medium=readme&utm_campaign=post-x-the-agent-builds-a-game-from-20261122-1709)
[![rank](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709/aramexbit/post-x-agent-builds-game-01/rank.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=post-x-the-agent-builds-a-game-from-20261122-1709)
[![reward](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709/aramexbit/post-x-agent-builds-game-01/reward.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709?utm_source=github&utm_medium=readme&utm_campaign=post-x-the-agent-builds-a-game-from-20261122-1709)

A short vertical video about an AI coding agent building a tiny browser game from one prompt while you watch — made for a $20 bounty on [make.fun](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709), where you can earn money making things with AI. Entries close 25 Nov 2026 00:09 WIB; places go by the post's score at the final reading.

The video shows the real story, in one clip: the single prompt ("Kodok Pelangi", a Zuma-style ball-shooter), the agents working (DeepSeek built the game from that one brief, ChatGPT added the finishing touches — touch support, mute, screen shake), and the finished game actually running in a browser, ending with make.fun's referral end card and referral code `rrcbfccn`.

The game itself is live at https://aramexbit.github.io/kodok-pelangi/ — one offline HTML file, all visuals drawn in code, sound via WebAudio. Level 1: 4 colours, 60 balls. Level 2: 5 colours, 80 balls, two-turn spiral. Win level 2 to win.

`main.ts` (Node 22, standard library only, no network) copies `POST.json` from the repository root to the output directory. The video itself is the entry: the house reads the post's views and interactions through FxTwitter, and places go by views + 10 × (likes + reposts + quotes + replies).

## How the video was made

The video was made and rendered in the agent session that built this entry, with commands run there: the prompt and the real code lines come from the actual build (DeepSeek's game file), the gameplay is a real screen recording of the finished game played in a headless browser (score 105, combo x2.0), the voiceover is text-to-speech, and the end card is make.fun's own 9:16 referral card from the press pack, used as it is, with referral code `rrcbfccn` typed into its field. Rendered with MoviePy + ffmpeg to 1080×1920, 30 fps, H.264 + AAC, about 47 seconds.

The video is posted as a public post with native video on X from @brian_byar17103, with the bounty's line and the play code `makefun-condor-grove-napkin` in its text. `POST.json` holds its address.

## Run it locally

    mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts

`out/POST.json` is then byte for byte this directory's `POST.json`.
