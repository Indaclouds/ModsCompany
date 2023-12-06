# LethalCompanyModder

This PowerShell script installs a selection of mods for LethalCompany.

It also includes the installation of BepInEx, a game patcher / plugin framework for Unity.

You don't need to install anything on your Windows system to run this script.

---

- [LethalCompanyModder](#lethalcompanymodder)
  - [How to use](#how-to-use)
    - [Basic installation](#basic-installation)
    - [Custom installation](#custom-installation)
      - [Install a curated preset of mods](#install-a-curated-preset-of-mods)
      - [Install a preset of mods from file](#install-a-preset-of-mods-from-file)
      - [Install for game host](#install-for-game-host)
    - [Upgrade](#upgrade)
  - [Curated presets of mods](#curated-presets-of-mods)
    - [`Default` preset](#default-preset)
    - [`Hardcore` preset](#hardcore-preset)
    - [`Experimental` preset](#experimental-preset)
  - [Check your files](#check-your-files)

---

## How to use

### Basic installation

To run ths script, follow these steps:

1. Open a PowerShell console.
2. Copy this _one-liner_ command in the console:

    ```powershell
    Set-ExecutionPolicy Bypass -Scope Process -Force; $Script = "$env:TEMP\LethalCompanyModder.ps1"; iwr "https://raw.githubusercontent.com/Indaclouds/LethalCompanyModder/main/LethalCompanyModder.ps1" -OutFile $Script; & $Script
    ```

3. Execute it.

It's as simple as that! 😄

### Custom installation

If needed, you can pass some parameters to the script:

```powershell
& .\LethalCompanyModder.ps1 <parameters>
```

#### Install a curated preset of mods

Install mods from a preser maintained by us on GitHub:

```powershell
& .\LethalCompanyModder.ps1 -Preset "Hardcore"
```

#### Install a preset of mods from file

Install mods from a preset defined in a file on your system:

```powershell
& .\LethalCompanyModder.ps1 -Preset "MyPreset" -File "./path/to/mods.json"
```

#### Install for game host

Install mods, including those required only by the game host:

```powershell
& .\LethalCompanyModder.ps1 -ServerHost
```

### Upgrade

If you need to update, re-run the script once again.

Mods and dependencies will be re-installed with the latest version.

## Curated presets of mods

### `Default` preset

_This is the selection of mods to be installed when no curated or custom preset is specified by the user._

- [MoreCompany](https://thunderstore.io/c/lethal-company/p/notnotnotswipez/MoreCompany/) by [notnotnotswipez](https://github.com/notnotnotswipez)
- [LateCompany](https://thunderstore.io/c/lethal-company/p/anormaltwig/LateCompany/) by [anormaltwig](https://github.com/ANormalTwig)
- [ShipLoot](https://thunderstore.io/c/lethal-company/p/tinyhoot/ShipLoot/) by [tinyhoot](https://github.com/tinyhoot)
- [HealthMetrics](https://thunderstore.io/c/lethal-company/p/matsuura/HealthMetrics/) by matsuura
- [TerminalApi](https://thunderstore.io/c/lethal-company/p/NotAtomicBomb/TerminalApi/) by [NotAtomicBomb](https://github.com/NotAtomicBomb)
- [Terminal Clock](https://thunderstore.io/c/lethal-company/p/NotAtomicBomb/Terminal_Clock/) by [NotAtomicBomb](https://github.com/NotAtomicBomb)
- [LBtoKG](https://thunderstore.io/c/lethal-company/p/Zduniusz/LBtoKG/) by Zduniusz
- [AlwaysHearActiveWalkies](https://thunderstore.io/c/lethal-company/p/Suskitech/AlwaysHearActiveWalkies/) by Suskitech

### `Hardcore` preset

- [MoreCompany](https://thunderstore.io/c/lethal-company/p/notnotnotswipez/MoreCompany/) by [notnotnotswipez](https://github.com/notnotnotswipez)
- [LateCompany](https://thunderstore.io/c/lethal-company/p/anormaltwig/LateCompany/) by [anormaltwig](https://github.com/ANormalTwig)
- [ShipLoot](https://thunderstore.io/c/lethal-company/p/tinyhoot/ShipLoot/) by [tinyhoot](https://github.com/tinyhoot)
- [LBtoKG](https://thunderstore.io/c/lethal-company/p/Zduniusz/LBtoKG/) by Zduniusz
- [LC API](https://thunderstore.io/c/lethal-company/p/2018/LC_API/) by [2018](https://github.com/u-2018)
- [Brutal Company](https://thunderstore.io/c/lethal-company/p/2018/Brutal_Company/) by [2018](https://github.com/u-2018)
- [SuperLandmine](https://thunderstore.io/c/lethal-company/p/phawitpp/SuperLandmine/) by phawitpp
- [AlwaysHearActiveWalkies](https://thunderstore.io/c/lethal-company/p/Suskitech/AlwaysHearActiveWalkies/) by Suskitech

### `Experimental` preset

- [MoreCompany](https://thunderstore.io/c/lethal-company/p/notnotnotswipez/MoreCompany/) by [notnotnotswipez](https://github.com/notnotnotswipez)
- [LateCompany](https://thunderstore.io/c/lethal-company/p/anormaltwig/LateCompany/) by [anormaltwig](https://github.com/ANormalTwig)
- [ShipLoot](https://thunderstore.io/c/lethal-company/p/tinyhoot/ShipLoot/) by [tinyhoot](https://github.com/tinyhoot)
- [HealthMetrics](https://thunderstore.io/c/lethal-company/p/matsuura/HealthMetrics/) by matsuura
- [TerminalApi](https://thunderstore.io/c/lethal-company/p/NotAtomicBomb/TerminalApi/) by [NotAtomicBomb](https://github.com/NotAtomicBomb)
- [Terminal Clock](https://thunderstore.io/c/lethal-company/p/NotAtomicBomb/Terminal_Clock/) by [NotAtomicBomb](https://github.com/NotAtomicBomb)
- [LBtoKG](https://thunderstore.io/c/lethal-company/p/Zduniusz/LBtoKG/) by Zduniusz
- [AlwaysHearActiveWalkies](https://thunderstore.io/c/lethal-company/p/Suskitech/AlwaysHearActiveWalkies/) by Suskitech
- [Solos Bodycams](https://thunderstore.io/c/lethal-company/p/CapyCat/Solos_Bodycams/) by CapyCat

## Check your files

If you would like to check your files after the installation, you can find them in the game directory.

The mods are located under the `BepInEx\plugins` directory.

![Check](https://github.com/Indaclouds/LethalCompanyInstallMods/assets/66850779/207efa58-edda-4922-bb98-15d1679b2a9d)
