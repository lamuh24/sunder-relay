# Sunder Relay

A Windows playtest of a cooperative action game made with Unreal Engine. Restore three relays, defeat the Hollow Crown, and reach the extraction lift.

**[Download the playable Windows ZIP](https://github.com/lamuh24/sunder-relay/releases/download/v0.1.1-playtest/SunderRelay-Windows-Playtest-0.1.1.zip)** (312 MB)

Version **0.1.1** fixes the invalid keyboard and mouse bindings in 0.1. Use this corrected build for play.

1. Download `SunderRelay-Windows-Playtest-0.1.1.zip` from the release assets.
2. Extract the entire ZIP into a new folder.
3. Open the extracted `SunderRelay` folder and double-click `Play.cmd`.
4. Choose an appearance with 1–4 and press Enter to begin.

The playable build is attached to the release. GitHub's automatic **Source code (zip)** download contains this repository's documentation, not the game. Unreal Editor is not needed to play.

| Input | Action |
| --- | --- |
| WASD | Move |
| Mouse | Aim |
| Left mouse | Fire blue energy bolts |
| Right mouse | Area pulse |
| Space | Dash |
| Q | Healing storm burst |
| Hold E near a fallen teammate | Revive |
| Esc | Quit |
| Enter after a result | Replay |

Stay within each relay perimeter for 40 seconds. After restoring all three, defeat the boss and reach the southern lift within 25 seconds.

For co-op, the host opens `HostCoop.cmd`; other players open `JoinCoop.cmd` and enter the host's reachable IPv4 address. The game uses UDP 7777. Four players were tested as separate processes on one computer. Play between different computers and over the internet remains unverified. Public matchmaking and an internet relay are not included.

This is an early playable prototype with one arena and mission, four warden appearances sharing a combat kit, and victory/defeat/replay. Automated complete solo, defeat, and localhost multiplayer checks passed on 0.1; those tests bypassed keyboard input and missed the binding defect. Normal play in 0.1.1 now confirms mission start, movement, mouse aiming, and repeated firing. All 17 input bindings pass Unreal's key validation. Laptop performance and the remaining individual ability inputs have not been separately verified. This is not a finished commercial game or a guarantee of bug-free play.

The build targets 64-bit Windows and DirectX 11 with a keyboard and mouse. It starts at 1280×720 with a 60 FPS cap. The included `READ_ME_FIRST.txt` has additional help. If a Microsoft runtime DLL is missing, the signed runtime installer is included under `Engine/Extras/Redist/en-us/`.

Archive size: **311,639,437 bytes**. SHA-256:

```text
37dad4b218e516dc4e82ad9b504f6bf501b4f071ef09b8d2158d9d83b519ea4c
```

The release also includes a laptop handoff prompt and an archive checksum file. Extract the complete named game archive, preserving all folders.
