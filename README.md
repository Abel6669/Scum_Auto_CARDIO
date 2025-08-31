# SCUM Cardio Macro (Windows EXE)

A lightweight, no-install macro GUI for SCUM that automates the ladder/stand cardio routine.

* **Single EXE** (no Python required).
* **Total ETA countdown** includes **gain + downtime**.
* Optional **auto-update**: checks the latest GitHub Release and can update in-app.


## Download

Grab the latest **`SCUM_Cardio_Macro.exe`** from the Releases page.
No installer, no extra files — just download and run.

* Latest: **[Download the EXE][releases-latest]**
* All versions: **[All Releases][releases]**

> SmartScreen may show “Windows protected your PC”. Click **More info → Run anyway**.


## Quick start

1. Run `SCUM_Cardio_Macro.exe`.
2. In **Inputs**, set your current/target STR and either **Over by (kg)** or **Carried (kg)**.
3. In **Timings**, adjust W/S hold, waits, and iterations (or use defaults).
4. Focus the SCUM window.
5. Click **Start** (or press **F5**).
6. Watch **ETA (total)** and the **Total/Gain** countdown.

**Keys sent by the macro** (default): `W`, `S`, `F`, `X`. You can pause (**F6**) or stop (**F7**) any time.


## What it does (under the hood)

* Runs W/S holds for **move gain**, adds a short **stand gain**, and includes neutral time (lay, waits).
* Computes rates from your **over/carry** and **loop split**, then converts to **real-world seconds** using your **sec per in-game minute**.
* The main countdown shows **total ETA** (including neutral/downtime), so what you see is real time to target.
* 

## Updating

You can update in either of two ways:

**A) In-app**

* Menu: **Help → Check for updates…**
* If a newer tag exists, the app downloads the latest `SCUM_Cardio_Macro.exe`, replaces itself, and restarts.

**B) Manual**

* Download the new EXE from **[Latest Release][releases-latest]** and replace your local file.

> Keep the filename **`SCUM_Cardio_Macro.exe`**. The updater expects the asset in Releases to match that name.


## Configuration & data

* Settings persist to:
  **Windows** → `%USERPROFILE%\.scum_cardio_macro.json`
* To reset: close the app and delete that file.


## Troubleshooting

* **“Nothing happens”**
  Make sure the **SCUM window is focused**. Macros send keys to the active window only.
* **Anti-virus flags the EXE**
  PyInstaller apps can trip heuristics. If downloaded from the Releases page, it’s the official build. You can verify the **SHA-256** below (if provided) or whitelist the EXE.
* **Keys don’t map correctly**
  If using a non-US keyboard layout, verify W/S/F/X are available. Adjust in-game bindings so those keys control the expected actions.
* **Updater says no updates**
  The app compares its version to the latest **Release tag**. Ensure the newest Release is tagged (e.g., `v1.2.3`) and published.


## Versioning & releases

* Versions follow `vMAJOR.MINOR.PATCH` (e.g., `v1.0.0`).
* The EXE in each Release is the **only** artifact you need.
* The app’s **About** dialog shows the running version.


## Security & privacy

* No telemetry. No external calls except optional **update check** against GitHub Releases.
* Use at your own risk; ensure macros comply with the game’s terms.


## Uninstall

Delete `SCUM_Cardio_Macro.exe` and `%USERPROFILE%\.scum_cardio_macro.json`.


