![image](https://github.com/Interkarma/daggerfall-unity/assets/10426244/4f176f9d-6332-47b3-a4d7-317ed8d6b38b)

# What is Daggerfall Unity?

Daggerfall Unity is an open source recreation of Daggerfall in the Unity engine created by [Daggerfall Workshop](http://www.dfworkshop.net).

Experience the adventure and intrigue of Daggerfall with all of its original charm along with hundreds of fixes, quality of life enhancements, and extensive mod support.

## Architecture

Daggerfall Unity is built on a modular architecture that leverages the power of the Unity engine while maintaining a clear separation from the original Daggerfall's game assets. This design ensures that the project remains a faithful recreation of the classic game while providing a flexible and extensible foundation for new features and mods.

The core of the application is a set of C# scripts, organized into a hierarchical structure that promotes code reusability and maintainability. The main components of the architecture are:

*   **Game Logic:** The `Assets/Scripts/Game` directory contains the primary gameplay logic, including character controllers, item systems, quest engines, and combat mechanics.
*   **API for Modding:** A dedicated `Assets/Scripts/API` provides a stable interface for modders to interact with the game's systems, allowing them to create new content and modify existing gameplay elements without altering the core source code.
*   **Asset Management:** The project uses Unity's Addressable Asset System to manage game assets, enabling efficient memory usage and allowing for the dynamic loading of assets at runtime.
*   **Daggerfall Asset Importers:** Custom importers and readers are used to load and process the original Daggerfall's game assets, such as textures, models, and sounds, from the `StreamingAssets` folder.
*   **Utility and Internal Systems:** The `Assets/Scripts/Utility` and `Assets/Scripts/Internal` directories contain a collection of helper classes and internal systems that support the main game logic, such as file I/O, data structures, and debugging tools.

This modular and extensible architecture has been instrumental in the success of Daggerfall Unity, fostering a vibrant modding community and enabling the continuous improvement of the game.

## Classic Daggerfall Plus

+ Cross-platform without emulation (Windows/Linux/Mac)
+ Retro graphics are boosted by modern engine and lighting
+ High resolution widescreen with classic style
+ Optionally play in retro mode 320x200 or 640x400 with VGA palettes
+ Optionally overhaul the graphics and gameplay with mods
+ Huge draw distances even without mods
+ Smooth first-person controls
+ Quality of life enhancements
+ Extensive mod support with an active creator community
+ Translation support via community mods

# Get Daggerfall Unity

Daggerfall Unity requires a free copy of DOS Daggerfall to run. This provides all necessary game assets such as textures, 3D models, and sound effects.

You can get a free copy of DOS Daggerfall from [Steam](https://store.steampowered.com/app/1812390/The_Elder_Scrolls_II_Daggerfall/) and a free copy of Daggerfall Unity from the [Releases](https://github.com/Interkarma/daggerfall-unity/releases) page. Then simply unzip the latest version of Daggerfall Unity to its own folder and point it to the DOS version. Daggerfall Unity will take care of everything else.

Here are a couple of links with more detailed steps to help you get started using either Steam or a cross-platform process.

+ [Using Steam Release of Daggerfall with Daggerfall Unity](https://github.com/Interkarma/daggerfall-unity/wiki/Using-Steam-Release-of-Daggerfall-with-Daggerfall-Unity)
+ [Installing Daggerfall Unity Cross Platform](https://github.com/Interkarma/daggerfall-unity/wiki/Installing-Daggerfall-Unity-Cross-Platform)

# System Requirements

## Building from Source

This guide provides instructions for building Daggerfall Unity from source on a Linux system.

### Prerequisites

*   **Unity Editor:** You will need Unity version **2019.4.40f1**. You can download it from the [Unity Download Archive](https://unity3d.com/get-unity/download/archive).
*   **Original Daggerfall Game Files:** Daggerfall Unity requires the original game assets from a classic Daggerfall installation. You can obtain a free copy of Daggerfall from [Steam](https://store.steampowered.com/app/1812390/The_Elder_Scrolls_II_Daggerfall/).

### Setup

1.  **Clone the Repository:**

    ```bash
    git clone https://github.com/Interkarma/daggerfall-unity.git
    cd daggerfall-unity
    ```

2.  **Place Daggerfall Game Files:**

    Copy the classic Daggerfall game files (the contents of the `DF/DAGGER` directory) into the `Assets/StreamingAssets/GameFiles` directory within the cloned repository.

### Building

1.  **Open the Project in Unity:**

    *   Launch the Unity Hub.
    *   Click the "Add" button and select the cloned `daggerfall-unity` directory.
    *   Open the project in the Unity Editor.

2.  **Build for Linux:**

    You can build the project using the command line. The following command will create a standalone 64-bit Linux build:

    ```bash
    /path/to/your/Unity/2019.4.40f1/Editor/Unity -quit -batchmode -projectPath . -buildLinux64Player Builds/DaggerfallUnity.x86_64
    ```

    Replace `/path/to/your/Unity/2019.4.40f1/Editor/Unity` with the actual path to your Unity editor executable. The build will be placed in the `Builds` directory.

Daggerfall Unity has the following system requirements. Please note that optional mods may substantially increase system requirements or cause game to become less stable.

### Minimum
* Operating system: Windows, Linux, MacOS
* Processor: Intel i3 (Skylake) equivalent
* Graphics: DirectX 11 capable with 1GB video memory and up-to-date drivers
* Memory: 2GB system RAM

### Recommended
* Operating system: Windows, Linux, MacOS
* Processor: Intel i5 (Skylake) equivalent
* Graphics: GTX 660 with 2GB video memory and up-to-date drivers
* Memory: 4GB system RAM

# Featured Mods

Daggerfall Unity has an active mod community with hundreds of incredible mods. It's impossible to feature them all, but here's a sampling of a few popular mods that represent a variety of mods the community has created. They range from graphical overhauls, to new quests, new guilds, adding new world areas, and changing game formulas and other behaviours.

## DREAM

![image](https://github.com/Interkarma/daggerfall-unity/assets/10426244/6a424f3c-f7f1-4def-82e9-98b6486dfc21)

The Daggerfall Remaster Enchanted Art Mod (DREAM) upgrades game assets including sound, music, videos & all graphics found in the game. It goes beyond a restoration and additionally fixes the old quirks, bugs and increases variety/fidelity everywhere possible.

[Link to DREAM on Nexus](https://www.nexusmods.com/daggerfallunity/mods/5)

## Quest Pack 1

![image](https://github.com/Interkarma/daggerfall-unity/assets/10426244/43688bd8-c3b0-42b5-bb64-066d6867ff66)

This quest pack offers 195 original new quests for Daggerfall Unity, mostly for the game's guilds.

[Link to Quest Pack 1 on Nexus](https://www.nexusmods.com/daggerfallunity/mods/2)

## Archaeologists

![image](https://github.com/Interkarma/daggerfall-unity/assets/10426244/282aa3a9-1662-49d9-9319-a9358775ea33)

Enhance Daggerfall Unity gameplay by making language skills more viable and adding a new guild to the game, called "The Archaeologists Guild". Their mission is to delve into the history of Tamriel and they're interested in all creatures and races who have lived or still live there. Joining gives access to locator devices to aid in dungeon delving.

[Link to Archaeologists on Nexus](https://www.nexusmods.com/daggerfallunity/mods/14)

## World of Daggerfall Project

![image](https://github.com/Interkarma/daggerfall-unity/assets/10426244/c3909d99-9ce4-4c41-8aaf-ee7dce49a6d7)

From the ashes of Daggerfall's past, experience the world of Daggerfall as originally envisioned. With glorious mountain tops that reach for the heavens, and countless new locations to explore.

[Link to World of Daggerfall Project on Nexus](https://www.nexusmods.com/daggerfallunity/mods/249)

## Finding My Religion

![image](https://github.com/Interkarma/daggerfall-unity/assets/10426244/995ae53d-eb99-451f-942c-931dd31dc85c)

Finding My Religion is a multi-release visual and gameplay overhaul of Daggerfall's religions. The current release is "Detailed Temples", which decorates and redesigns the temples' according to the worshipped deity's sphere of influence. Julianos boasts a bigger library than others, Kynareth has an indoor garden, Mara has a birthing room and more. Each temple have been expanded downwards,  with priests' quarters and additional rooms for all service members. They also feature a crypt where people of importance have been buried.

[Link to Finding My Religion on Nexus](https://www.nexusmods.com/daggerfallunity/mods/344)

## Physical Combat And Armor Overhaul

![image](https://github.com/Interkarma/daggerfall-unity/assets/10426244/35bc2fb2-5b3d-401d-b3cb-806a59241014)

Instead of increasing chance to avoid an attack completely, armor now reduces the damage you take, based on the material as well as the type of attack. Skills now determine most of your chance to avoid attacks, including many more features.

[Link to Physical Combat And Armor Overhaul on Nexus](https://www.nexusmods.com/daggerfallunity/mods/76)

## Links

+ [Daggerfall Unity Nexus](https://www.nexusmods.com/daggerfallunity) - *Discover more mods for Daggerfall Unity*
+ [Lysandus' Tomb Discord](https://discord.gg/rn95kxPGpg) - *Join an active growing community*
+ [Daggerfall Workshop](http://www.dfworkshop.net/) - *Follow the development of Daggerfall Unity*
+ [Workshop Forums](http://forums.dfworkshop.net/) - *Join the forum community*
+ [Reddit](https://www.reddit.com/r/daggerfallunity) - *Join the Daggerfall Unity subreddit*
+ [Twitter](https://twitter.com/gav_clayton) - *Follow lead developer on Twitter for more news*
