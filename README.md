# NBT Tooltip (Fork)

A Minecraft (Fabric) mod that shows an item's **NBT / data components** directly in its tooltip, and lets you **copy them to the clipboard**. Handy for datapack, command and map makers.

> **This is a fork.** Original mod by **Zabi94**, previously updated by **tricrotism**. This fork by **flyingfinger1** keeps it working on current Minecraft versions — **1.21.8 through 26.2** — including the Yarn → Mojang-mappings migration that Minecraft 26.x requires.
>
> Licensed under **MIT** (see [`LICENSE`](LICENSE), original copyright retained). Upstream: <https://github.com/tricrotism/NBTTooltip>

## Downloads

There is one build per Minecraft generation (each on its own branch). Grab the matching jar from the [Releases](https://github.com/flyingfinger1/NBTTooltip/releases) page:

| Minecraft | Branch | Mappings | Java |
|---|---|---|---|
| 1.21.8 | `fabric/1.21.8` | Yarn | 21 |
| 1.21.9 – 1.21.11 | `fabric/1.21.11` | Yarn | 21 |
| 26.1.x | `fabric/26.1` | Mojang | 25 |
| 26.2 | `fabric/26.2` | Mojang | 25 |

> Minecraft 26.x ships unobfuscated and needs **Java 25**; Fabric discontinued Yarn after 1.21.11, so the 26.x builds use Mojang mappings.

## Requirements
- **Fabric Loader** + **Fabric API**
- **Cloth Config** — bundled inside the jar, no separate download needed
- **Mod Menu** — optional, only for the in-game config screen (on 26.x currently a beta). Without it, edit `config/nbttooltip.json` directly.

## Usage
- By default the NBT tooltip appears when **advanced tooltips** are enabled — press **F3 + H** — or set *Trigger Type* to `ALWAYS_ON` in the config.
- Default keybinds (rebindable under Controls): **Copy** = Right Arrow, **Toggle** = Left Arrow, **Scroll** = Up / Down.
- Hold **Shift** to pause auto-scroll, **Alt** to scroll faster, **Ctrl** to show only the NBT (hiding the rest of the tooltip).
- Presentation (friendly / colored / JSON) and copy format are configurable.

## Building
- 1.21.x branches need **JDK 21**, the 26.x branches need **JDK 25**.
- `./gradlew build` → output in `build/libs/`.
- CI builds every branch on push (see the `build` workflow under Actions).

## Credits
- **Zabi94** — original author
- **tricrotism** — previous fork / updates
- **flyingfinger1** — this multi-version fork (1.21.8 – 26.2)

Released under the MIT License.
