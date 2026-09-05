# Sunder Relay

A Windows playtest of a cooperative action game made with Unreal Engine. Restore three relays, defeat the Hollow Crown, and reach the extraction lift.

**[Download the playable Windows ZIP](https://github.com/lamuh24/sunder-relay/releases/download/v0.1.0-playtest/SunderRelay-Windows-Playtest-0.1.zip)** (312 MB)

1. Download `SunderRelay-Windows-Playtest-0.1.zip` from the release assets.
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

This is an early playable prototype with one arena and mission, four warden appearances sharing a combat kit, and victory/defeat/replay. Automated complete solo, defeat, and localhost multiplayer checks passed. Manual input testing and laptop performance remain unverified. This is not a finished commercial game or a guarantee of bug-free play.

The build targets 64-bit Windows and DirectX 11 with a keyboard and mouse. It starts at 1280×720 with a 60 FPS cap. The included `READ_ME_FIRST.txt` has additional help. If a Microsoft runtime DLL is missing, the signed runtime installer is included under `Engine/Extras/Redist/en-us/`.

Archive size: **311,641,261 bytes**. SHA-256:

```text
756360c36be7fe7a388b0cfdfe6b5d4e22813bc8eae34fd4b434222008202634
```

The archive has been extracted with Windows PowerShell `Expand-Archive`, and all 46 game files passed their SHA-256 checks. The release also includes a laptop handoff prompt and an archive checksum file.
