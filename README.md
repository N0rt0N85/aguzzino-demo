# Aguzzino: the Doom shareware on the Sega Saturn, on line

Aguzzino is a game engine for the Sega Saturn. This demo plays the nine maps of
the Doom shareware episode, with its music and sounds, alone or with bots, and
with other players over the internet through the Saturn's NetLink modem.

## Download

On the **Releases** page:

| File | What it is |
|------|------------|
| `AguzzinoNetLink-Mednafen-Windows-SW24.zip` | Mednafen 1.32.1 with an emulated NetLink modem, the disc and its launchers, for Windows |
| `AguzzinoNetLink-Mednafen-macOS-SW24.zip` | the same for macOS (Apple Silicon only) |
| `AguzShareware24.zip` | the disc alone (`.cue` + `.bin`), for a real Saturn or another emulator |
| `AguzShareware18Taisen.zip` | the SW18 build of the game for two Saturns joined by the link cable (see below) |

## What you need

A Saturn BIOS dump of your own (`mpr-17933.bin`, or `sega_101.bin` for Japan).
We cannot provide it. Put it in `mednafen_home/firmware`, then double-click
`play_online.bat` (Windows) or `play_online.command` (macOS). The `README.txt`
inside each package has the details.

## Playing on line

The packages call the Aguzzino team's relay, which is in France. In the game:
MULTIPLAYER, set PLAY to ON LINE, choose the mode and the map, press START. A
game starts when 4 players are in, or 30 seconds after the last one arrived.
A bot joins a game that has a free place, one bot per game at most.

Far from Europe, a game is smoother through a relay near its players. The
`relay` folder of each package has the relay program, its settings and the
steps to run your own, with bots too (`relay/README.txt`).

## Two Saturns by the link cable

`AguzShareware18Taisen.zip` is the SW18 build of the game, whose on line modes go through
the link cable between the rear serial ports of two Saturns instead of the
NetLink: two players, with no relay, no modem and no PC. Each Saturn needs its
own copy of the disc. On both: MULTIPLAYER, set PLAY to ON LINE, choose the
mode and the map, press START, the two within a minute.

**Nobody has tried it on a Saturn yet.** Two emulated Saturns joined by an
emulated cable played it without a fault; the cable's wiring, the levels and
the timing of a real console are not checked. Its `README.txt` says what was
tested. Please tell us how it went in the Issues.

## Known limits

- On line, everyone needs the same disc: the calling screen says `DISC SW24`.
- Nobody can join a game already running.
- On line, the game has only been played on emulators so far.

## Licences

- Mednafen is GPL-2.0-or-later, by the Mednafen Team (https://mednafen.github.io/).
  The NetLink modem emulation is a modification of it under the same licence:
  its source is in the `source` folder of each package.
- The relay (the `relay` folder) is under the MIT licence (`relay/LICENSE.txt`).
- Doom is by id Software.
