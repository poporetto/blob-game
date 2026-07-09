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
- **Size titles**: Crumb → Snacker → Muncher → Chonker → Glutton → **CAKE LORD** (crown included). Each rank pays +200.
- **Air combos**: every extra treat eaten in a single hop multiplies its points.
- **Belly flop**: a big blob landing hard sends a shockwave that hoovers up nearby floor treats.
- **Sugar Rush**: an 8-treat streak makes you rainbow — treats magnetize toward you and growth doubles.
- **Chili peppers** are the one thing on the menu you must not eat: sour face, shrinkage, streak lost.
- The **TUMMY** bar always drains — faster the bigger you are. Starve and the blob deflates. Size is glory, but it's rent.

## Tech

Single-file vanilla JS + canvas at 240×320 internal resolution, integer-physical-pixel scaling (`image-rendering: pixelated`), procedural sprites and squash-and-stretch animation, WebAudio sound. No dependencies — portrait-first for an easy mobile port.
