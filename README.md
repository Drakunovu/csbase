# CSBase
A modern, ready-to-deploy Counter-Strike 1.6 server base. This repository is optimized for quick startup and includes the latest ReHLDS ecosystem binaries pre-configured.

## ⚠️ OS Requirements & Windows Users
**This repository contains Linux binaries (`.so`) only.** It will not run natively on Windows command prompt or PowerShell.

* **Linux Users:** You can run this natively.
* **Windows Users:** You **MUST** use [WSL (Windows Subsystem for Linux)](https://learn.microsoft.com/en-us/windows/wsl/install) to run this server.

## 📦 Prerequisites
To run the server binaries properly, you need the 32-bit GCC support library (`lib32gcc-s1`).

### Installing dependencies
Run the command corresponding to your Linux distribution:

**Debian / Ubuntu / WSL (Ubuntu)**
```bash
sudo apt update
sudo apt install lib32gcc-s1
````

**Arch Linux**

```bash
sudo pacman -S lib32-gcc-libs
```

**CentOS / Fedora (RHEL)**

```bash
sudo dnf install libgcc.i686
```

## ⚙️ Mandatory Configuration

Before starting the server, you must generate a secure salt for the **Reunion** module. This ensures player SteamIDs are hashed uniquely and securely.

1.  Open the configuration file: `csbase/cstrike/reunion.cfg`
2.  Navigate to **Line 97** to find the setting `SteamIdHashSalt`.
3.  Replace the default value with a long, random alphanumeric string (no symbols).

### Salt Generator Command

You can run this command in your terminal to generate a secure, 64-character alphanumeric string automatically:

```bash
cat /dev/urandom | tr -dc 'a-zA-Z0-9' | fold -w 64 | head -n 1
```

**Example of how it should look in the file:**

```ini
SteamIdHashSalt = aW8s7d6f5g4h3j2k1l0m9n8b7v6c5x4z3a2s1d0f9g8h7j6k5l4
```

## 📂 Included Content

This base includes the following pre-installed modules and binaries:

|    Module   |   Version  | Description |
|:-----------:|:----------:|:------------|
|    ReHLDS   |   e999171  | Reverse-engineered HLDS engine |
|  ReGameDLL  |   f63ad67  | Fixed and improved CS game logic |
|  Metamod-R  | v1.3.0.149 | Metamod optimized for ReHLDS |
|  AMXX v1.10 | build 5467 | Scripting platform for plugins |
|    ReAPI    |   ab961d6  | API for advanced AMXX interaction |
|   Reunion   |  v0.2.0.13 | Protocol manager (Non-Steam support) |
|   Revoice   |  v0.1.0.34 | Voice chat fix for newer clients |
| ReAuthCheck |   v0.1.6   | Security module (Anti-Fake/Proxy) |
|  ReSemiClip |   v2.4.3   | Teammate collision fix |