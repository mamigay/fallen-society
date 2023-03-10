![FS Header](img/FS_Header.png)

**IMPORTANT:** This is a Fallout 4 modlist that contains adult content. To access this content you need to be 18 years of age (in most countries), 21 in other. Please make sure that you fullfill the legal specifications of your country.

**For general support and talk about the modlist, join the Fallen Society Discord:**

[![DiscordButton](img/DiscordButton.png)](https://discord.gg/cprgvBUCpH)

# ToC
- [What is Fallen Society?](#what-is-fallen-society)
- [Before you start](#before-you-start)
  - [Hardware requirements](#hardware-requirements)
  - [DLC \& Creation Club Content](#dlc--creation-club-content)

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
