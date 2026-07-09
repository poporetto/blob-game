# Blob Bakery — Sugar Rush 🍰🍫🍬

A pixel-art game about a bouncy purple blob with one goal in life: eat every dessert in sight and get **absolutely enormous**.

## Play

Open `index.html` in a browser, or serve it:

```sh
python3 -m http.server 8642
# → http://localhost:8642
```

## Controls

- **Hold** (mouse or touch): the blob squats down and charges power; an arc shows where it will fly.
- **Release**: BOING. The blob leaps toward your pointer, bouncing off walls and floor.

## How it works

- Cakes, chocolate bars, candies and donuts spawn on the floor and floating in the air.
- Touch a treat → the blob's mouth gapes open, the treat gets sucked in, chomp-chomp, and a gulp bulge travels down its body as it **grows**.
- **Size ranks**: Crumb → Snacker → Muncher → Chonker → Glutton → **CAKE LORD** (crown included). Each rank pays +200; the HUD badge shows progress to the next one.
- **Air combos**: every extra treat eaten in a single hop chain (bounces included) multiplies its points, capped at x5.
- **Marshmallow trampolines** drift around mid-air — bounce off them to extend a hop and keep the combo chain alive.
- **Belly flop**: a big blob landing hard sends a shockwave that hoovers up nearby floor treats.
- **Sugar Rush**: an 8-treat streak (watch the pips fill under the rank badge) makes you rainbow — treats magnetize toward you and growth doubles.
- **Flying donuts** flap around on little wings and must be chased.
- **Golden cakes** are rare, sparkly, worth 150 points, and refill the tummy completely.
- **CAKE RAIN!** every ~40 seconds the sky dumps treats for a few seconds; leftovers melt away.
- **Quests** rotate in the bottom-left chip ("EAT 3 CHOCS", "DO A COMBO x3", "BELLY FLOP x2"...) — each pays +400 and a tummy top-up.
- **Chili peppers** are the one thing on the menu you must not eat: sour face, shrinkage, streak lost. They get more common the bigger you are.
- The **TUMMY** bar always drains — faster the bigger you are. Starve and the blob deflates. Size is glory, but it's rent.
- Game over shows your run stats: treats eaten, best combo, belly flops, quests done, peak rank.

## Tech

Single-file vanilla JS + canvas at 240×320 internal resolution, integer-physical-pixel scaling (`image-rendering: pixelated`), procedural sprites and squash-and-stretch animation, WebAudio sound. No dependencies — portrait-first for an easy mobile port.
