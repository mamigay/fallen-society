![FS Header](img/FS_Header.png)

**IMPORTANT:** This is a Fallout 4 modlist that contains adult content. To access this content you need to be 18 years of age (in most countries), 21 in other. Please make sure that you fullfill the legal specifications of your country.

**For general support and talk about the modlist, join the Fallen Society Discord:**

[![DiscordButton](img/DiscordButton.png)](https://discord.gg/cprgvBUCpH)

# ToC
- [What is Fallen Society?](#what-is-fallen-society)
- [Before you start](#before-you-start)
  - [Hardware requirements](#hardware-requirements)
  - [DLC \& Creation Club Content](#dlc--creation-club-content)
- [Installation](#installation)
  - [Preparation](#preparation)
    - [Microsoft Visual C++ Redistributable Packages](#microsoft-visual-c-redistributable-packages)
    - [Page file setup](#page-file-setup)
    - [Setup your Shader Cache](#setup-your-shader-cache)
    - [Disable Steam Overlay](#disable-steam-overlay)
    - [Set game language to English](#set-game-language-to-english)
    - [Change Steam's Updating Behavior](#change-steams-updating-behavior)
    - [Clean current Fallout 4 installation](#clean-current-fallout-4-installation)
    - [Install Fallout 4](#install-fallout-4)
    - [Start Fallout 4](#start-fallout-4)
  - [Wabbajack](#wabbajack)

# What is Fallen Society?
A NSFW Fallout 4 modlist that aims to be as immersive as possible. If you want large overhauls and tons of new quests, than this is **not** the list for you. This one aims to modify and fix almost every aspect of the base game, add some new locations, weapons etc. and add a spicy portion of NSFW mods on top. Your goal is to survive and to rebuild society in a harsh environment.

# Before you start
Please read carefully and check every requirement here:

## Hardware requirements
I have a decent setup at home with the following specs:
- CPU: Intel(R) Core(TM) i7-10700K CPU
- RAM: 96GB DDR4
- GPU: NVidia RTX 3080 (12GB VRAM)

So that should give you an idea of what you need (except for the RAM maybe. 32GB should be more than enough).

I play at 4k resolution (3840 x 2160) and have constant 60FPS in most areas. Of course there are some drops here and there but nothing major and nothing below 40FPS for more than a second. The list should be very performant.

You should have at least ```180 GB``` of free space on an SSD (better -> m.2 SSD) for the installation and an additional ```80 GB``` for the downloads. So you would need to have around ```260 GB``` of free space. If you insist on installing this list on an HDD, than prepare yourself for painfull and hard installation! You are warned.

## Accounts
You need the following accounts to download this list:
- Nexus Premium Account (you can use free, but it would take ages)
- LoversLab Account
- Moddingham Account (needed for the lates AAF version)

## DLC & Creation Club Content
You need all Fallout 4 DLC except for the official HD texture pack. **DON'T INSTALL IT!**
Creation Club content is and will not be supported.

# Installation
At this point you should have read everything that came before und didn't skip anything. The next section requires a lot of attention so read carefully.

## Preparation

### Microsoft Visual C++ Redistributable Packages
This is hard requirement for MO2 to operate. You may already have it installed, if not, download the x64 version under "Visual Studio 2015, 2017 and 2019) here:
[Download Visual C++ Redistributable Package.](https://docs.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170)

### Page file setup
Fallout 4 modlists need a large amount of memory purely because of the amount of *stuff* in them - especially modlists on the larger side or with a lot going on. For the best experience, you should setup a pagefile of at least **20GB** - yes, even if you have a million GB of RAM. To setup your pagefile;

1. Hold down the *LEFT* Windows key and press **R**
2. Type in `systempropertiesadvanced` in the run box and then press ENTER
3. Under the "Performance" option, click the "Settings..." button
4. Switch to the "Advanced" tab
5. Under "Virtual Memory", click the "Change..." button
6. Uncheck `Automatically manage...` if it's checked
7. Select your *fastest* SSD in the list of drives
8. Check "Custom Size"
9. Set `Initial Size` to 20480
10. Set `Maximum Size` to 20480 also
    1.  *Note: you can set this up to 40000 if you have the space, this will let the pagefile expand to as large as 40GB*
11. Press the "Set" button
12. Press OK
13. Press APPLY and then OK
14. Restart your PC to apply the pagefile setting

### Setup your Shader Cache
Driver defaults from Nvidia and AMD for shader cache size is limited to 4GB. Being this small can lead to rare crashes in heavily modified Fallout 4 installs. Increasing the shader cache size is done via the Nvidia Control Panel (I assume the same for AMD users is true also but I don't have AMD hardware to check with). 

*These instructions are Nvidia specific as it is the hardware I have.*

1. Open the NVidia Control Panel
2. Head to `Manage 3D Settings`
3. Scroll down in `Global Settings` to find the `Shader Cache Size` option
4. Set the Shader Cache to *at least* 10GB
5. Done

![Shader Cache](img/ShaderCache.png)

### Disable Steam Overlay
The Steam overlay is known to cause issues when using ENBs. I recommend you turn it off to be sure that it doesn't interfere in any way and you can do so by heading into Steam, right clicking on Fallout 4 in your game library and clicking **Properties** > **General** > **Deselect "Enable Steam Overlay while in-game"**.

### Set game language to English
Wabbajack and some/most of the modding tools out there only support English language versions of games. Setting the language to English in Steam will stop issues like Wabbajack file verification failures when installing. As with disabling the overlay, right click on Fallout 4 in your game library and click **Properties** > **Language** > **Select English**.

### Change Steam's Updating Behavior
If for some reason Bethesda decide to release an update for Fallout 4, everything will probably break. Well, not *everything* but something will definitely break until mods can be updated to suit. To stop this from happening, you need to tell Steam that you only want to update when you tell it to. You can do this by right clicking on Fallout 4 in your game library and clicking **Properties** > **Updates** > **Change Automatic Updates to "Only update this game when I launch it"**. Whilst you're in here, it's also recommended to disable Steam Cloud too.

### Clean current Fallout 4 installation
If you have not yet installed Fallout 4, you can skip this part.

1. Right click on Fallout 4 in your game library and click **Properties** > **Local Files** > **Browse**. 
2. Uninstall the game via Steam - right click on Fallout 4 in your game library and click **Manage** > **Uninstall**.
3. Check the explorer window for any left over files - if there are any, delete them.
4. Open Windows start menu/search and type in `%LOCALAPPDATA%`.
5. Delete the Fallout 4 folder.
6. Head to `Documents\My Games` and delete the Fallout 4 folder.

### Install Fallout 4
Once you've done the steps above, you can now set Steam to download Fallout 4 again but ***do not*** install Fallout 4 to a protected folder, such as `Desktop`, `Downloads` or `Program Files` of any kind. It's best to create a new, dedicated folder for it using the Steam Library function somewhere on the root of your drive such as `C:\SteamLibrary`. A lot of people have a dedicated secondary drive for their games, keeping the OS install separate; using this secondary drive will also work.

### Start Fallout 4
That's right - start the game. You need to let the game do its initial start up jobs such as creating registry entries and generating default config files. Once you've gotten to the main menu you can close the game again.

## Wabbajack
Installing the list is straight forward, Wabbajack will do most of the heavy lifting for you - you only have to tell it where to put stuff.

Set the installation location to a folder on the root of a drive, something like `C:\WoD`. Do not install it to one of the protected folders as mentioned earlier. The download location will have likely been filled in for you too - ensure it matches the directory you set for the installation location, or if you have multiple Fallout 4 modlists installed, use a common download folder - this will stop you from having to redownload common mods across multiple modlists. 

Before you hit **GO**, a quick tip:

*To get the best performance with Wabbajack, it is recommended that you have the install folder for Wabbajack, the modlist folder and the downloads folder on an SSD; ideally the same SSD.* After the installation is complete, you can move the downloads folder to a storage HDD or other storage medium to save space on your game installation drive. It's not recommended to allow your drive to exceed 90% of its storage space used - Windows Explorer will show a red bar under your drive if you do go over 90% so you need to be sure that you have enough space on your installation drive so that you won't exceed this 90% storage level.

Once you have everything set in Wabbajack, hit **GO** and let it do its thing. It might take a while as there is a fair bit to download and the speed of this will depend on your internet performance as well as your CPU in the later stages for hashing and unpacking the downloads.
