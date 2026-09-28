# Easier Hydrogen

NeoForge 1.21.1 addon for Mekanism. Adds simple **Chemical Oxidizer** recipes
(one item in, one chemical out) so common chemicals are easy to make.

| Chemical | Input (1 item) | Output |
|---|---|---|
| Hydrogen | Snowball | 100 mB |
| Hydrogen | Ice | 400 mB |
| Hydrogen | Snow block | 400 mB |
| Hydrogen | Packed ice | 800 mB |
| Hydrogen | Blue ice | 1600 mB |
| Hydrogen | Water bucket | 1000 mB |
| Oxygen | Any leaves (`#minecraft:leaves`) | 100 mB |
| Chlorine | White dye | 100 mB |
| Sodium | Dried kelp | 100 mB |
| Ethene | Apple | 100 mB |
| Ethene | Sugar cane | 100 mB |
| Sulfur dioxide | Gunpowder | 50 mB |
| Hydrofluoric acid | Fluorite (`#c:gems/fluorite`) | 100 mB |
| Antimatter | Ender pearl | 100 mB |
| Antimatter | Eye of ender | 200 mB |
| Antimatter | Nether star | 1000 mB |
| Plutonium | Netherite scrap | 100 mB |
| Polonium | Prismarine crystals | 100 mB |
| Nuclear waste | Rotten flesh | 100 mB |
| Fissile fuel | Uranium ingot | 100 mB |
| Superheated sodium | Blaze rod | 100 mB |
| Steam | Wet sponge | 1000 mB |
| Sulfur trioxide | Blaze powder | 100 mB |
| Sulfuric acid | Magma cream | 100 mB |
| Spent nuclear waste | Poisonous potato | 100 mB |
| Uranium oxide | Uranium dust | 100 mB |
| Uranium hexafluoride | Uranium crystal | 100 mB |
| Water vapor | Sponge | 500 mB |
| Hydrogen chloride | Sea pickle | 100 mB |
| Clean copper slurry | Raw copper | 500 mB |
| Clean gold slurry | Raw gold | 500 mB |
| Clean iron slurry | Raw iron | 500 mB |
| Clean lead slurry | Raw lead | 500 mB |
| Clean osmium slurry | Raw osmium | 500 mB |
| Clean tin slurry | Raw tin | 500 mB |
| Clean uranium slurry | Raw uranium | 500 mB |
| Helium | Glowstone dust | 100 mB (only if Mekanism: Sun is installed) |
| Helium | Glowstone block | 400 mB (only if Mekanism: Sun is installed) |

## Crafting table (antimatter pellets)
Shaped, 3x3: eyes of ender in the corners, crying obsidian on the edges, nether star in the center -> **2 antimatter pellets**.

## Alloyer (Mekanism: Sun)
| Inputs | Output |
|---|---|
| 1 Electrum ingot + 1 Lapis lazuli + 100 mB helium | 2 Raw uranium |
| 1 Gold ingot + 1 Iron ingot + 100 mB helium | 2 Electrum ingots (replaces the silver recipe) |

## Build on GitHub
1. Push the **contents** of this folder (so `build.gradle` is at the repo root) to a GitHub repo.
2. Open the **Actions** tab. The `Build` workflow runs on every push.
3. Download the jar from the run's **Artifacts** section (`easier-hydrogen`).
4. Drop it in your `mods` folder next to Mekanism 10.7.x.

## Build locally
Needs JDK 21 and Gradle 8.10+: `gradle build` -> `build/libs/`.

## Tweak or add recipes
Recipes live in `src/main/resources/data/mekanism/recipe/oxidizing/<chemical>/`.
Copy any file, change the `input` item/tag and the `output` id/amount.
