# SpaceTube

A free, original neon tube shooter with a head nod to the classic 80s vector arcade shooter. You ride the rim of a glowing wireframe web and blast everything that climbs up the lanes toward you. Sixteen web shapes, five kinds of climbers, a boss every fifth web, power-ups, and an upgrade shop between webs.

**Play it in your browser:** https://nbwillcox.github.io/SpaceTube/

Everything is generated in code: the webs, claw, enemies and bosses are vector-drawn on the fly, and all sound effects and the title tune are synthesized with the Web Audio API. There are no image or audio files and no build step. A sibling of [SpaceGalaShooter](https://github.com/nbwillcox/SpaceGalaShooter), [SpacePac](https://github.com/nbwillcox/SpacePac) and the rest of the series.

## Controls

| Action | Keys |
| --- | --- |
| Step around the rim | `←` `→` or `A` `D`, mouse wheel, or move the mouse (the claw follows the pointer) |
| Fire (hold) | `Space`, `W`, `↑` or left mouse button |
| Zapper | `X`, `Z`, `Shift`, `S`, `↓` or right mouse button |
| Pause | `P` or `Esc` |

A gamepad also works (d-pad or stick to steer, `A` to fire, `B` / `X` / `RB` for the zapper, Start to pause).

### On a phone or tablet

Play in portrait. Slide a thumb left or right anywhere on the screen to step the claw around the rim (one lane per short slide). The cannon fires by itself, and **ZAP** is the screen-clearing zapper. The pause button opens the menu. The on-screen controls appear on touch devices automatically; Settings has size, opacity and a left-handed layout. Use your browser's *Add to Home Screen* to install it as a full-screen app.

## Gameplay

- **The goal:** shoot every climber in the web. When the last one dies, you warp to the next web, and then visit the upgrade shop.
- **The climbers:**
  - **Flipper** (red) climbs while flipping from lane to lane, then runs along the rim to catch you.
  - **Tanker** (purple) splits into two flippers when it is shot or reaches the top.
  - **Spiker** (green) lays a spike up its lane. Shoot the spike to shorten it: if you finish the web standing in a lane with a spike, the warp kills you.
  - **Fuseball** (yellow) rides the spokes between lanes and zaps you if it reaches the rim next to you.
  - **Pulsar** (cyan) charges up and electrifies its whole lane. Do not be standing in it.
- **Bosses** arrive on every fifth web: The Maw, The Hive and The Prism. Shoot through the armor plates to open a lane, then hit the glowing core. Boss bolts are telegraphed: when a lane flashes, leave it. Broken plates slowly grow back.
- **Power-ups** drop from kills and wait on the rim for you to step into their lane: **R** rapid fire, **S** spread shot, **P** piercing, **H** shield, **Z** a zapper charge, and **1UP**.
- **The zapper** clears the whole screen once per charge, and hurts bosses a lot.
- **Upgrade shop:** credits come from your score and from clearing webs. Spend them between webs on fire rate, magazine size, claw speed, piercing rounds, longer power-ups, a starting shield, a starting zapper and extra lives.
- **Lives and score:** 3 lives, an extra life every 25,000 points. Local top-10 high scores are kept in your browser.

## Run it locally

Open `index.html` in a browser, or serve the folder with any static server, for example `python -m http.server`. Test flags: `?level=N` starts on web N, `?god=1` makes you immune, `?touch=1` forces the touch controls on a desktop.

## License

[CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/): free to play, share and remix for non-commercial use, with a link back to https://github.com/nbwillcox/SpaceTube. SpaceTube is an original game inspired by the arcade golden age; it uses no names, art, sounds or code from any commercial game.
