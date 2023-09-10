# Bonelab Mod Manager [![Rust](https://github.com/valentinegb/bonelab_mod_manager/actions/workflows/rust.yml/badge.svg)](https://github.com/valentinegb/bonelab_mod_manager/actions/workflows/rust.yml)

Keeps your installed Bonelab mods synced with your subscribed mod.io mods.

<img width="858" alt="Screenshot 2023-09-08 at 4 38 43 PM" src="https://github.com/valentinegb/bonelab_mod_manager/assets/35977727/b2c810b3-586b-4103-ad96-f1bc449abf30">

## Features

- Multi-platform
  - macOS
  - Linux
  - Windows
- PC and Quest mod support
- Parallel downloads
- Installs subscribed mod.io mods
- Installs PC mods directly into Bonelab installation
- Updates mods
- Removes unsubscribed mods
- Built with [Rust](http://rust-lang.org)

You can see this project's backlog [here](https://github.com/users/valentinegb/projects/4).

## How to Use

1. Download the appropriate file from the [latest release](https://github.com/valentinegb/bonelab_mod_manager/releases/latest) (or [a pre-release](https://github.com/valentinegb/bonelab_mod_manager/releases)) for your OS.
2. Launch the program, by double clicking or other method.
  - If you're on Windows, you may be prevented from launching the program by a popup warning you that the program is not safe.
    It is, and if you don't believe me you can check the code yourself. To launch the program anyway, click "More info" then "Run anyway".
3. On your first time running, you will be prompted to sign in to mod.io. Use the arrow keys to select your method of signing in then press enter.
4. If you are on Windows, you will be prompted whether you would like to install PC mods or Quest mods.
5. After that, the program will do the rest for you! Sit back, relax, and watch as all your mods are downloaded and installed.
6. Next time you want to sync your installed mods, just run the program again.

## Quest Mod Installation Path

PC mods are installed directly into a PC Bonelab installation, but Quest mods must be manually put onto your headset. Quest mods are installed in a directory dependent on your OS.

macOS: `~/Library/Application Support/com.valentinegb.bonelab_mod_manager/Mods`

Linux: `~/var/lib/bonelab_mod_manager/Mods`

Windows: `%AppData%/bonelab_mod_manager/Mods`

I know, it isn't ideal having to move the mods from this folder to your headset,
but it's on the roadmap for the mod manager to do that for you, it will in the future!

## Configuring Concurrent Downloads

By default, Bonelab Mod Manager will install 4 mods at a time. This is configurable however since hardware can differ drastically. To change the maximum number of concurrent downloads, set the `BMM_CONCURRENT_DOWNLOADS` environment variable.
