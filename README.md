# Base FPS Game

A minimal, extendable starter first-person shooter project for Unreal Engine — works with UE4.27 (Chaos) and Unreal Engine 5. Use this repository as a learning base, rapid prototype, or starting point for a full game.

---

## Why this exists
- There are few open-source, ready-to-run Unreal FPS starter projects. This repo provides a small, well-organized base you can extend.
- Focused on being easy to understand and modify so contributors can add features quickly.

---

## Features
- Basic FPS framework: movement, camera, and input
- Built for UE4.27 (Chaos) and compatible with UE5
- Clean layout intended for extending weapons, AI, levels, and mechanics

---

## Requirements
- Unreal Engine 4.27 (with Chaos) or Unreal Engine 5 (any compatible version)
- Git
- Git LFS recommended if the repo contains large binary assets

---

## Quick start
1. Clone the repository:
   ```bash
   git clone https://github.com/sdcardbro123/base-fps-game.git
   cd base-fps-game
   ```
2. (If used) Install and fetch Git LFS assets:
   ```bash
   git lfs install
   git lfs pull
   ```
3. Open the project:
   - Double-click the `.uproject` file to open in the Editor, or
   - In the Epic Games Launcher click the project ykh...

---

## If Epic Games Launcher doesn't show the project
If the Epic Games Launcher does not list your project under "My Projects", try these steps — the Launcher sometimes fails to detect new project folders automatically.


Manual Windows fix (edit the Launcher config)
0. Quit Epic Games Launcher completely (right-click the tray icon → Exit). If you don't quit the launcher, changes to the config may be overwritten when it closes.
1. Navigate to:
   ```
   C:\Users\<your-username>\AppData\Local\EpicGamesLauncher\Saved\Config\Windows
   ```
2. Open the file:
   ```
   GameUserSettings.ini
   ```
3. At the end of the file, add a [Launcher] section (or add CreatedProjectPaths lines under the existing [Launcher] section) listing parent folders that contain your projects. Example:
   ```
   [Launcher]
   CreatedProjectPaths=D:/ParentFolderOfYourProject
   CreatedProjectPaths=D:/DifferentParentFolderOfYourOtherProject
   ```
   Note: Add the parent folder(s) that contain your .uproject folder(s). Do not add the project folder itself — add its parent directory.
4. Save the file and reopen Epic Games Launcher. The projects in the added folders should now appear under "My Projects".

---

## Common troubleshooting
- Assets or plugins fail to load:
  - On Windows, right-click the `.uproject` → Generate Visual Studio project files, then re-open the project.
  - On macOS/Linux, use the appropriate GenerateFiles script for your platform.
- Project opens in the wrong engine version:
  - Right-click the `.uproject` → Switch Unreal Engine version, then choose the correct engine.
- Missing content after clone:
  - Ensure Git LFS is installed and run `git lfs pull`.
- Crashes or build errors:
  - Check the Output Log in the Editor for plugin/asset errors, disable or remove incompatible plugins, and verify engine compatibility.

---

## Contributing
Contributions are welcome! Suggested workflow:
1. Fork the repository.
2. Create a descriptive branch: `feature/my-new-weapon` or `fix/bug-description`.
3. Make focused changes and include a short description of what and why.
4. Open a pull request describing the change and any testing steps.

For bug reports and feature requests, open an issue and include reproduction steps, engine version, and logs if possible.

---

## Roadmap / Ideas
- Add example weapons and pickup system
- Simple AI enemies and wave-spawning
- UI elements (health, ammo, score)
- Example level and tutorial

If you want to see any of these features prioritized, open an issue or submit a PR.

---

## License
MIT LICENSE
---

## Contact
Maintainer: @sdcardbro123

Enjoy building — and feel free to open issues or PRs with improvements!
