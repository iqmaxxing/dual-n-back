# Dual n-back rules on IQMAXXING

These are the default rules of [Dual N-Back](https://iqmaxxing.org/dual). Every one of them can be checked against a run's exported trials (Stats, Data, Trials CSV).

## The task

Each trial shows a square in one of 8 cells around the centre of a 3 by 3 grid and speaks one letter from C, H, K, L, Q, R, S and T. On every trial you answer two questions: is this square where the square was N trials back, and is this letter the one spoken N trials back. Press the position key for a square match and the audio key for a letter match. Press nothing when neither matches.

## A run

- **Length.** N lead-in trials, which are never judged, then 20 judged trials (Jaeggi 2008's 20 + N). 30, 35, 40, 50, 60 and any length up to 100 in fives can be set.
- **Pace.** A trial starts every 3.0 seconds. The square and the letter come on together and the square stays lit for 500 ms. Pace can be set from 1.3 to 5.0 seconds in steps of 100 ms.
- **Matches.** 30% of the judged trials are a match in each stream, dealt rather than rolled, so a 20-trial run always has 6 per stream. 10% of the judged trials are a match in both streams at once.
- **Lures.** About one non-matching trial in eight repeats the item from N minus 1, N plus 1 or 2N back, so it feels familiar without being a match.
- **No easy repeats.** A non-matching trial never repeats the trial just before it.
- **Seeded.** Every run is dealt from a seed, so the same seed deals the same run on every device.

## The score

Each stream is scored on its own: hits divided by hits, misses and false alarms. Correct rejections earn nothing, so pressing on every trial does not score well.

## The level

- **Up.** When both streams score 80% or better, the result suggests the next level.
- **Down.** After three runs in a row whose pooled score is under 50%, the result suggests the level below.
- The result suggests, and you choose: Again takes the suggestion.

## Other settings

Shifted (executive) n-back, Variable N, d′ progression, the long cue, match and lure rates, and the 9-cell board change the task and keep records of their own. The runs counted in `data/` use none of them. [Advanced n-back](https://iqmaxxing.org/theory/advanced-n-back) explains each.
