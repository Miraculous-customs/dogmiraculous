# Dog Miraculous — Forge 1.20.1

A standalone Dog Miraculous mod for Minecraft Forge 1.20.1 and Java 17.

## Dog Miraculous

- Kwami: Barkk
- Jewel: collar worn in the Curios necklace slot
- Transformation: `Barkk, On the Hunt!`
- Detransformation: `Lay Down.`
- Power: `Fetch!`
- Weapon: throwable ball
- Transformation key: `Y`
- Detransformation key: `U`
- Power key: `X`
- Restore Active form: `H`
- Open the Active collar menu: `M`

The normal transformation lasts five minutes. After timing out, Barkk must be
recharged with Minecraft food. One hundred successful Fetch uses permanently
unlock grown-up mode and remove the five-minute transformation limit.

## Implemented

- Active and Camo collar states
- Supplied Active and Camo collar mesh models rendered through Forge OBJ
- Curios necklace support
- Custom Curios neck rendering for both collar forms
- Hero-name menu
- Throwable Dog ball
- Supplied 3D mesh ball model for held and thrown rendering
- Recall of marked dropped items
- Crouch-targeting of another player's held item
- Dog suit overlay that preserves the player's normal skin
- Dog ears and Blockbench/GeckoLib model resources
- Speed IV, Jump Boost IV, Regeneration IV, and Strength IV while transformed
- Five-stage transformation timer HUD
- Original armor restoration after detransformation
- Food recharge
- Animated GeckoLib Barkk companion who accepts any edible Minecraft food
- Grown-up progression and operator override
- Optional Nastia's Miracle Stones compatibility through shared Forge tags

## Required APIs

- GeckoLib `4.8.4+`
- Curios `5.14.1+1.20.1`
- Kleider's Custom Renderer `7.4.0+`

## Operator command

```text
/dogmiraculous <username> grown_up true
```

Use `false` to restore the normal five-minute limit.

## Build

Use Java 17 and run:

```bash
./gradlew build
```

The compiled JAR is written to `build/libs/`.

Editable Dog models and textures are stored under `model-work/`.

The included GitHub Actions workflow also builds the playable JAR automatically
whenever the source is pushed to the `main` branch.
