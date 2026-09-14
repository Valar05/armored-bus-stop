# Armored Bus Stop

A one-file, mobile-first battlefield driving toy descended from **Last Convoy**, **Long Haul**, and the infantry contribution in **Through the Slit**.

## Thesis

The player gets no action buttons.

The player drives an armored personnel carrier. Steering, throttle, braking, terrain, drift, and arrival geometry decide when and where carried infantry can act. Enter a marked bus stop slowly enough and the rear doors open automatically. The people inside are the capability layer.

```text
DRIVE
-> ARRIVE
-> DOORS OPEN
-> PEOPLE INHERIT THE GEOMETRY
-> THEY FIGHT
-> DRIVE AGAIN
```

## Controls

Touch:

- left thumb: steering
- right thumb: vertical throttle / brake / reverse surface
- no attack button
- no dismount button

Keyboard:

- `W` / Up: throttle
- `S` / Down: brake, then reverse
- `A` / `D` or Left / Right: steering

## Mechanics in this first specimen

- vehicle facing, travel heading, and momentum are distinct enough to create gravel-like skew;
- grip changes by firm ground, gravel, and mud;
- arrival at a bus stop requires low speed, not an action press;
- passenger fireteams spawn from the rear hatch, so carrier orientation changes the geometry they inherit;
- infantry move to cover and fight automatically;
- enemies pressure deployed teams and the carrier;
- the APC can ram by driving, but has no player-fired weapon;
- three stops and three fireteams are enough for a complete run.

## Run

Open `index.html` directly, or serve the folder with any static server.

```sh
python -m http.server 8787
```

Then open `http://127.0.0.1:8787/`.

No build step and no external assets are required.
