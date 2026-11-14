# DAVEN JUMP

### Hop through the channels. Dodge the moss. Get home.

> Daven is a hedgehog who got stuck inside a retro TV. Every channel is a haunted, mossy forest
> full of villains, mud and spiky chestnuts that would really like him to go away.
> All he wants is his den, and maybe a few acorns on the way.

Made for **Hack Club Haven**

---

## The story

Nobody knows how Daven ended up inside the TV. One second he was minding his own business
in the leaves, and the next he was on Channel 1 with a moss monster staring at him.

The good news: the TV has five channels, and his den is at the end of the last one.
The bad news: every channel is wetter, weirder or more upside-down than the one before.
The only way through is up, down, and bouncing back.

---

## How to play

- **Run and jump** across the forest.
- **Collect acorns.** They're your money, and they stay with you across channels.
- **Bounce** off mushrooms and moss mounds to reach high places.
- **Stomp** on villains from above. Touching one from the side hurts.
- **Fall in a pit?** You'll pop back to the start, no hard feelings.
- **Reach the den** to finish the channel.
- **Beat the Moss Monster** (four stomps) to unlock the den on the last channel.

### Controls

| Action | Keyboard | Hardware (optional) |
| --- | --- | --- |
| Move | `←` `→` or `A` `D` | |
| Jump | `Space`, `↑` or `W` | |
| Volume up | `]` or `=` | VOLUME knob, turn clockwise |
| Volume down | `[` or `-` | VOLUME knob, turn counter-clockwise |
| Mute / unmute | `M` | VOLUME knob, push |
| Reset the channel | `R` | RESET knob, push |

---

## The channels

| # | Channel | What's special |
| --- | --- | --- |
| 1 | **Acorn Path** | The basics. Pits, a mushroom, and your first villain. |
| 2 | **Leaf Hop** | Low gravity, leaf platforms, and bounces that go very high. |
| 3 | **Muddy Slide** | The mud has no friction. Plan your stops carefully. |
| 4 | **Backwards Burrow** | The autumn wind spun the forest around. Left is right now. |
| 5 | **Moss Monster's Den** | The boss fight. The den stays locked until the monster is defeated. |

---

## Who's trying to stop you

| Enemy | What it does | How to beat it |
| --- | --- | --- |
| **Moss villain** | Walks the ground, turns at ledges, and chases you when it sees you. | Stomp it twice. |
| **Moss Monster** (boss) | Big, grumpy, four lives, and it guards the den. | Stomp it four times. |
| **Chestnut** | Spiky, bobs up and down, and can't be squished. | Don't touch it. Time your jumps. |

---

## Acorns

Acorns are the currency of the forest. They spin, bob and sparkle, and every one you grab
adds to your wallet at the top right of the screen.

Your wallet is kept across channels and resets. Resetting a channel won't let you farm the
same acorns twice, so grab them carefully and keep moving.

## Bouncy things

- **Mushrooms**: a normal bounce.
- **Moss mounds**: a super bounce that launches you high.
- **Stomping an enemy**: bounces you back up in the air, so chain your stomps if you can.

---

## The TV

The whole game lives inside a retro TV:

- A **VOLUME** knob and a **RESET** knob along the bottom, which turn as you use them.
- A **power light** that turns red when the TV is muted.
- **Speaker grilles** on the bezel.
- **Scanlines**, a curved screen and a little flicker.
- **Static** when you switch channels, reset, or finish a level.

Every sound is generated in the game itself, so there are no audio files to download.

---

## Run it in 30 seconds

There's nothing to install. The whole game is one file.

1. Download **`index.html`**.
2. Open it in your browser by double-clicking it, or in VS Code right-click the file and choose
   **Open with Live Server** (install the *Live Server* extension first if you don't have it).
3. Press any key to switch on the TV.

Browsers only allow sound after a key press, so the first key you press is the one that turns
the TV on.

---

## Optional: a hardware remote

Want the knobs to be real? The volume and reset controls can be two rotary encoders
on a **Raspberry Pi Pico** running CircuitPython. The included `code.py` makes the Pico
send the same keys as the keyboard, so the game doesn't need to know it's a remote.

- **Encoder 1 (volume)**: `A` → GP2, `B` → GP3, `SW` → GP4. Turn for volume, push to mute.
- **Encoder 2 (reset)**: `SW` → GP8. Push to reset the channel.
- Both common pins go to GND.
- Copy `code.py` to the Pico, and put the `adafruit_hid` library in the `lib` folder.

---

## Built with

- Plain **HTML, CSS and JavaScript**, with the game drawn on a `<canvas>`.
- The **Web Audio API** for sound effects.
- No frameworks, no build step and no internet connection needed.
- One `index.html` file with all the art embedded in it.

---

## Credits

- **Hedgehog sprites**: *Pixel Art Hedgehog* by **DustDFG**, licensed under
  [CC-BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).
  Original: <https://dustdfg.itch.io/pixel-art-hedgehog>.
  If you share changed versions of these sprites, share them under CC-BY-SA 4.0 too.
- **Mushroom and tiles**: **Kenney**'s Pixel Platformer, [CC0](https://creativecommons.org/publicdomain/zero/1.0/)
  (<https://kenney.nl>). No credit needed, but it's appreciated.
- **Ground, stone ledges, mounds and backgrounds** (night sky, cemetery, tombstones, dead tree):
  **Anokolisa**, free to use, with credit appreciated.
  <https://www.patreon.com/Anokolisa>
- **Acorn and Moss Monster sprites**: `[add the artist or source here]`

---

## Ideas for later

- More channels, and maybe a channel where the TV is upside-down the whole time.
- More villains with new moves.
- A save file, so your acorns survive closing the tab.
- Touch controls for phones.

---

## License

`[add your license here, for example MIT]`

The art is credited above and keeps its own licenses.
