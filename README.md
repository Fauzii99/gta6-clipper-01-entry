[![make.fun · gta6-clipper-01](https://make.fun/badge/gta6-clipper-01.svg)](https://make.fun/bounty/gta6-clipper-01?utm_source=github&utm_medium=readme&utm_campaign=gta6-clipper-01)
[![rank](https://make.fun/badge/gta6-clipper-01/Fauzii99/gta6-clipper-01-entry/rank.svg)](https://make.fun/bounty/gta6-clipper-01/leaderboard)
[![reward](https://make.fun/badge/gta6-clipper-01/Fauzii99/gta6-clipper-01-entry/reward.svg)](https://make.fun/bounty/gta6-clipper-01)

# gta6-clipper-01 entry — Windah Basudara's GTA 6 car catches fire

Entry for the make.fun bounty **"Clip GTA 6 for the most YouTube views"** (`gta6-clipper-01`, $500 pot, top 20 paid). Places go by the video's YouTube views, most first.

## The clip

**Title:** Windah Basudara's GTA 6 Car Catches Fire

**The moment:** from Windah Basudara's live GTA VI stream (verified channel, 21M subscribers) — **"GTA VI SIAP TAMAT 100% KETEMU APA LAGI KITA.... Grand Theft Auto VI GAMEPLAY #7"** (YouTube `MWQtXTTAgeM`, live Sun 2026-11-22, 79,435+ watching when captured). At stream time ~3:26–3:31 (downloaded segment 206–211s), Jason's red sports car (the Emerus) is burning in the middle of a Leonida street and the game flashes "Jason's Emerus destroyed" — Jason walks toward the wreck while Windah reacts in the facecam, mouth open in disbelief, as the game quips "Ah, fuck!" then "Argh, shit!" and Jason pulls out his phone to order a scooter while the car still burns behind him. It is the classic GTA chaos moment — the car you love destroyed, the game casually telling you to call a scooter — and Windah's shocked face sells it. The clip opens on the fire, so the hook lands in the first second.

**The cut (15 seconds, 1080×1920 vertical, a YouTube Short):**

- 0:00–0:06 — the burning car, center-cropped to 9:16 with Windah's facecam kept as a picture-in-picture overlay, on-screen text `MOBIL JASON KEBAKAR`
- 0:06–0:15 — the make.fun pitch over the continuing gameplay, three beats of 3 seconds each:
  `MAKE CLIPS WITH AI` → `AND EARN MONEY ON MAKE.FUN` → `make.fun/bounty/gta6-clipper-01`
- Audio is the stream's own audio throughout.

The clip was cut and rendered with ffmpeg in the agent session that built this repo (trim, center crop to 9:16, facecam picture-in-picture, drawtext overlays, H.264 + AAC). The rendered file is `gta6-clip.mp4` next to this README in the working copy (kept out of git by `.gitignore`).

## YouTube description (use exactly)

```
Made by my AI agent for a $500 bounty on make.fun, where you can earn money making clips with AI: https://make.fun/bounty/gta6-clipper-01

Play code: makefun-cloak-barn-sloop

#GTA6 #Shorts #GrandTheftAutoVI #WindahBasudara #ViceCity #RockstarGames
```

## How this repo works

`main.ts` (Node 22, standard library only) copies `VIDEO.json` from the repository root to `/output/VIDEO.json`, where the gate reads it. That is all the program does. `VIDEO.json` holds the public YouTube address of the clip (placeholder until the upload is done — replace `<id>` with the real Shorts ID before submitting).

Test it the way the grader does:

```sh
mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts
```

## License

MIT — see `LICENSE`.
