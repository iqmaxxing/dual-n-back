# dual-n-back

Open numbers and the exact rules of dual n-back as it is played on [IQMAXXING](https://iqmaxxing.org/dual), a free dual n-back trainer for the web, iPhone, iPad and Android.

This repository holds data and a written spec. It holds no game code. To play, go to **[iqmaxxing.org/dual](https://iqmaxxing.org/dual)**.

## What is here

| file | what it is |
| --- | --- |
| [RULES.md](RULES.md) | How a run is dealt, timed and scored, and how the level moves |
| [data/summary.csv](data/summary.csv) | Players, runs and hours counted, and the dates they cover |
| [data/passed.csv](data/passed.csv) | How many players have passed 2-back, 3-back, and 4-back or higher |
| [data/highest_level_passed.csv](data/highest_level_passed.csv) | Each player by the highest level they have passed |
| [data/runs_to_pass.csv](data/runs_to_pass.csv) | Runs and days it took to pass a level: lower quartile, median, upper quartile |
| [data/streams_by_level.csv](data/streams_by_level.csv) | Miss and false alarm rates per stream at each level, and which stream was weaker |
| [data/pace.csv](data/pace.csv) | The share of runs that passed, by pace |

The same figures, with charts, are on [Dual n-back, by the numbers](https://iqmaxxing.org/dual-n-back-data). The site counts them again every six hours; this repository is a dated copy, refreshed by hand.

## How the numbers are made

- A run counts when it is a dual n-back run saved since 27 September 2026, the day matches became a fixed 30% of each stream, played with the standard matches and lures on the 8-cell board. Every pace and run length counts, from the website and the apps.
- Left out: runs from a challenge link, and runs with Shifted, Variable N, d′ progression, custom matches, lures or cue, or the 9-cell board. Guided and practice runs are never saved. The site owner's own account is not counted.
- A player is one history: a browser's, or an account's once signed in. No name or account is read. The same person on two devices without an account counts as two players.
- A player has passed a level when a run at it ended with both streams at 80% or better.
- `miss_rate` is misses over the matches dealt, and `false_alarm_rate` is false alarms over the non-matches, averaged with each player counted once.
- A figure about fewer than 10 players is left blank. A count that would let a smaller group be worked out by subtraction is rounded.
- These are people who chose to train on one site, many of them for a single run. They are not a norm for anyone else, and a level describes this task alone.

## Licence

The data and the text in this repository are under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Credit "IQMAXXING, iqmaxxing.org".
