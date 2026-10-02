# Neon Nightfall

Play here : https://mdhasibul35.github.io/neon-nightfall/

A colorful first-person zombie wave survival game that runs in any modern browser. No install and no build step: it is a single `index.html` file.

## Play

Open `index.html` in a browser, or play the hosted version on GitHub Pages (see below).

### Controls

**Computer**

| Key | Action |
| --- | --- |
| W A S D / arrow keys | Move |
| Mouse | Aim |
| Left click | Shoot |
| Shift | Sprint |
| R | Reload |
| E | Buy a weapon / open a door / drink a tonic |
| Q, 1, 2, mouse wheel | Swap weapon |
| M | Mute |
| Esc or P | Pause |

**Phone / tablet**

- Left thumb: move (push all the way to sprint)
- Right side drag: aim
- Buttons: Fire, R (reload), Use, Swap, II (pause)

## How to play

- Zombies climb out of glowing portals. Each wave brings more, and they get tougher.
- Hits earn 10 points, kills 60, headshot kills 100.
- Spend points on wall weapons:
  - Fizz SMG: 750
  - Confetti Cannon: 1200
  - Prism Ray: 2500 (its beam passes through enemies)
- Buying a weapon you already own refills its ammo for half price.
- Open the **Sky Garden** for 1000 points. This also activates new portals.
- Drink **Tough Tonic** (2000 points) to raise max health to 175.
- Kills sometimes drop power-ups:
  - Prism Bomb clears the field.
  - Gold Rush doubles points.
  - Refill gives full ammo.
  - Sugar Rush makes you faster.

## Publish it free with GitHub Pages

1. Create a new public repository on GitHub, for example `neon-nightfall`.
2. Upload `index.html` and `README.md` to the root of the repository. Use **Add file → Upload files**, then **Commit changes**.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to **Deploy from a branch**. Choose the `main` branch and the `/ (root)` folder, then **Save**.
5. Wait a minute or two, then refresh the page. Your game link appears at the top. It looks like:
   `https://YOUR-USERNAME.github.io/neon-nightfall/`

Share that link with anyone and they can play.

## Tech

- [three.js](https://threejs.org/) r128, loaded from cdnjs. Players need an internet connection.
- Fonts: Bungee and Chakra Petch from Google Fonts.
- All sounds are generated in code with the Web Audio API, so there are no audio files.
- The best wave is saved in the player's browser with `localStorage`.
