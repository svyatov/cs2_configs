# Counter-Strike 2 config

svyatov's personal [CS2 autoexec](autoexec.cfg), adapted from the [original CS:GO config](https://github.com/svyatov/csgo_configs). The numeric keypad buys weapons and grenades. The mouse wheel selects a gun, and holding Z extends the crosshair for grenade lineups.

## Install and verify

1. In Steam, open the properties for Counter-Strike 2. Under **Installed Files**, select **Browse**.
2. Open `game/csgo/cfg` in the game folder. Back up any existing copies, then copy `autoexec.cfg` and `practice.cfg` there.
3. Start CS2 and open the developer console. Run `exec autoexec`. Look for `svyatov autoexec.cfg loaded` to confirm the file loaded.

If the console is disabled, turn on **Enable Developer Console** in the game settings.

On a Mac with the Steam library in its default location, `./copy.sh` copies both files. For a custom library, use the manual steps above.

## Practice

Start a local practice map, join a team, and run `exec practice` in the console. The round restarts with $60,000, five grenades, and no bots. You can buy anywhere. Guns have unlimited reserve ammo and still need reloading.

| Key | Practice action |
| --- | --- |
| F4 / F5 | Toggle the eight-second flight trail / repeat the last grenade throw. |
| F6 / F7 | Toggle bullet impact markers / penetration details. |
| F8 | Toggle the grenade landing preview. |
| X / J | Toggle flight / zoom in to inspect a lineup. |
| Comma / period | Add a CT bot / T bot. |
| P / K | Place a bot at your crosshair / remove all bots. |

Run `practice_end` to disconnect and restore this config's normal controls. If you use personal bindings for comma, brackets, P, or K, add them to your autoexec so it restores them too.

The [practice config](practice.cfg) also includes the original workshop arrow shortcuts as comments. Enable them for maps that provide those commands.

## Controls

| Key | Action |
| --- | --- |
| X / E | Open the buy menu / interact. |
| Keypad | Buy the item shown in the keypad diagram in [autoexec.cfg](autoexec.cfg). Equip the weapon in your team's loadout first. |
| Left / Right arrow | Buy armor and a helmet, or armor alone if needed / buy a defuse kit. |
| Up / Down arrow | Buy HE and smoke with two flashes (Up) or one flash and a fire grenade (Down). |
| Mouse wheel up / down | Select the primary weapon / pistol. Each direction falls back to the knife if the slot is empty. |
| Mouse 4 / Mouse 5 / V | Select a flashbang / smoke / fire grenade. |
| Z | Hold for a lineup crosshair. Release to restore the normal crosshair. |
| B | Press to select the bomb if carried. Release to drop it and switch back to a gun. |
| Left Alt / Insert / F1 | Hold to talk / toggle voice chat / temporarily silence teammates during a clutch. |
| Tab / period | Hold Tab for the scoreboard and full telemetry. Press period to toggle full readings between scoreboard checks. |
| F10 | Disconnect immediately. |

## Customize

Edit [autoexec.cfg](autoexec.cfg) to change the settings or bindings. For a closer radar view, increase `cl_radar_scale`. To resize the radar panel, change `cl_hud_radar_scale`. The `-nadecrosshair` alias sets the normal crosshair length, gap, and outline at startup and when you release Z.

After editing the repository copy, copy it into the game folder again. Press `/` in game to reload it.
