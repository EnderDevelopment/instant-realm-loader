# Minecraft Bedrock Performance Behavior Pack

Instant Realm Loader is a Minecraft Bedrock behavior pack for Bedrock 26.50+ that provides an optional performance mode for the current dimension. It reduces background simulation by disabling random ticks and natural mob spawning, and it works in the Overworld, Nether, and End when enabled separately in each dimension.

## Install

1. Import the `.mcpack` file by opening it with Minecraft.
2. Open the settings for the world where you want to use the pack.
3. Open **Behavior Packs**.
4. Select **Instant Realm Loader** and activate it.
5. Enable cheats if Minecraft requires command permissions.
6. Enter the world.
7. Run this command in the dimension where you want to enable performance mode:

```text
/function quickload_enable
```

To develop or install manually, copy the pack folder containing `manifest.json` and the `functions` folder into Minecraft's `development_behavior_packs` directory.

## Use

Enable performance mode in the current dimension:

```text
/function quickload_enable
```

This sets:

- `randomTickSpeed` to `0`
- `doMobSpawning` to `false`

These settings can stop crop growth, leaf decay, fire spread, and natural mob spawning while enabled. They may reduce background simulation after the world opens, but they can change normal gameplay.

Disable performance mode and restore common defaults in the current dimension:

```text
/function quickload_disable
```

This sets:

- `randomTickSpeed` to `3`
- `doMobSpawning` to `true`

Run the enable or disable function separately in the Overworld, Nether, and End because gamerules apply to the dimension where the command runs.

The pack cannot remove Minecraft's loading screen, force terrain to load instantly, preload Nether or End chunks, guarantee five-second loading, or guarantee zero lag. Initial world loading and terrain generation are controlled by Minecraft and the device running the game.

The pack targets Minecraft Bedrock 26.50+. Test it after game updates because command behavior and pack requirements may change.

To create an `.mcpack` file manually, zip the folder contents containing `manifest.json` and `functions`, then rename the `.zip` extension to `.mcpack`.

---

More Minecraft mod projects by EnderDevelopment: https://github.com/EnderDevelopment

Project page: https://dash.enderdevelopment.com/community/85a26bc7-a7cd-43ed-afd5-2b0642227947?utm_source=github&utm_medium=readme&utm_campaign=auto_publish&utm_content=85a26bc7-a7cd-43ed-afd5-2b0642227947
