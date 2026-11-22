[![make.fun · gta6-clipper-01](https://make.fun/badge/gta6-clipper-01.svg)](https://make.fun/bounty/gta6-clipper-01?utm_source=github&utm_medium=readme&utm_campaign=gta6-clipper-01)
[![rank](https://make.fun/badge/gta6-clipper-01/Fauzii99/gta6-clipper-01-entry/rank.svg)](https://make.fun/bounty/gta6-clipper-01/leaderboard)
[![reward](https://make.fun/badge/gta6-clipper-01/Fauzii99/gta6-clipper-01-entry/reward.svg)](https://make.fun/bounty/gta6-clipper-01)

# gta6-clipper-01 entry — Windah Basudara achieves Criminal Profile Professional

Entry for the make.fun bounty **"Clip GTA 6 for the most YouTube views"** (`gta6-clipper-01`, $500 pot, top 20 paid). Places go by the video's YouTube views, most first.

## The clip

**Title:** Windah Basudara Achieves Criminal Profile Professional in GTA 6

**The moment:** from Windah Basudara's live GTA VI stream (verified channel, 21M subscribers) — **"GTA VI SIAP TAMAT 100% KETEMU APA LAGI KITA.... Grand Theft Auto VI GAMEPLAY #7"** (YouTube `MWQtXTTAgeM`, live Sun 2026-11-22). At stream time 1:20:30–1:21:02, Windah opens the pause menu and checks his stats: Jason Duval's **"CRIMINAL PROFILE: PROFESSIONAL"** (yellow icon) pops on the stats screen, and he celebrates, fist raised. Then Lucia's stats show she is **also** "CRIMINAL PROFILE: PROFESSIONAL" — both protagonists are Professional — the game resumes on the boat, and he opens the map (Port Gellhorn / Draper Island). It is the cleanest kind of GTA moment: the game itself hands you a rank, and the creator's face sells it. The clip opens on the boat, so the hook lands in the first seconds, and the "PROFESSIONAL" reveal gets a zoom-in at 1:20:43.

**The cut (34 seconds, 1080×1920 vertical, a YouTube Short):**

- Split-screen reaction format: Windah's facecam big and centered on top, gameplay below, bold caption bar at the boundary — `POV: Windah jadi kriminal profesional`. Facecam and gameplay are cropped from the same frame, so the top and bottom always show the same moment.
- 0:00–0:05 — boat lead-in
- 0:05–0:09 — pause menu, JASON/LUCIA select
- 0:09–0:16 — Jason's stats, "CRIMINAL PROFILE: PROFESSIONAL", fist celebration — with a zoom-in on the "PROFESSIONAL" text at 1:20:43 (clip ~12.5–14.5s), then zoom back out
- 0:16–0:21 — Lucia's stats, also "PROFESSIONAL", back to select
- 0:21–0:29 — the game resumes on the boat
- 0:29–0:34 — the map (Port Gellhorn / Draper Island)
- 0:25–0:34 — the make.fun pitch over the last 9 seconds of the actual footage (boat + map), three beats of 3 seconds each:
  `MAKE CLIPS WITH AI` → `AND EARN MONEY ON MAKE.FUN` → `make.fun/bounty/gta6-clipper-01`
- Audio is the stream's own audio throughout, in sync with the picture (cut from the same take).
- Source is genuine 720p (recovered from the stream's HLS segments after it went private), upscaled to 1080×1920 with lanczos + sharpening.

The clip was cut and rendered with ffmpeg in the agent sessions that built this repo (single continuous take, split-screen crop from the same frame, zoompan zoom, drawtext overlays, H.264 + AAC). The rendered file is `gta6-clip.mp4` next to this README in the working copy (kept out of git by `.gitignore`).

## YouTube description (use exactly)

```
Windah Basudara Achieves Criminal Profile Professional in GTA 6

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
