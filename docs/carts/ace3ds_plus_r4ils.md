# Ace3ds+ / R4iLS / clones

The list of carts that this page applies to can be found [here](https://gitHub.com/ds-homebrew/flashcard-archive), though I'll copy-paste them here too:

* Ace3DS+
* Ace3DS X
* \#\#\# in 1 combo cart
* r4isdhc.com.cn carts
* r4isdhc.hk 2020+ carts
* r4li.com carts
* r4infinity.com 2
* r4ixds.com 2014 white version
* woodr4isdhc.com carts
* (possibly) DSTTi.cc - Behaves like an Ace3ds+ where it only activates when an SD card is inserted, though it has not been tested with the ace3ds+ kernel. IF you have this cart, please open an issue and let me know if it works!
* Unlabelled cart with a red PCB - Note: There are different types of unlabelled red cart, see here to differentiate between them: (URL PLACEHOLDER)

!> DO NOT install YSMenu on these carts. While some of them may appear similar to the timebomb clones from r4isdhc.com, none of these carts can use YSMenu

These carts will use the Ace3ds+ wood 1.62 kernel, this is not R4 wood 1.62.
Ace3ds+ wood is based on an old version of R4 wood, it's not based on R4 wood 1.62 as the name might suggest.
It is missing some anti-piracy patches but nonetheless is good for game compatibility!

## Setup (Ace3ds+ Wood 1.62)

1. Download Ace3ds+ wood from here: [https://flashcard-archive.ds-homebrew.com/Ace3DS+_R4iLS/Ace3DS+_R4iLS_Wood_R4_1.62.7z](https://flashcard-archive.ds-homebrew.com/Ace3DS+_R4iLS/Ace3DS+_R4iLS_Wood_R4_1.62.7z)
1. Extract the Ace3ds+ wood archive
1. Copy the kernel files to the root of your micro SD card

On the root of your micro SD card, you should see:

* \_rpg folder
* \_DSMENU.dat file
* \_DS\_MENU.dat file

### Twilight menu ++

This cart supports twilight menu ++!
You can install it by following these instructions: [https://wiki.ds-homebrew.com/twilightmenu/installing-flashcard](https://wiki.ds-homebrew.com/twilightmenu/installing-flashcard)

While I don't really use twilight menu ++ on my flashcards, if you want to play some [*supported* dsiware](https://github.com/DS-Homebrew/TWiLightMenu/blob/master/universal/include/compatibleDSiWareMap.h), it's definitely an option to look into! Best part about Twilight menu ++ is that it is in active development, meaning that more dsiware will be supported in the future!

Twilight menu ++ also bundles in some emulators for other consoles, see the list here: []()

### AOS 2.13

This kernel is just Ace3ds+ wood with bundled emulators. It is no longer maintained and so the emulators bundled with it could be outdated.

I'd recommend using Twilight Menu ++ instead if you want the bundled emulators. If you still want to use AOS 2.13, follow these instructions:

1. Download the AOS 2.13 repack from here: [link](https://github.com/DS-Homebrew/flashcard-archive/raw/d1b3a804b9ce76540b3f94c2a916740f7435dc43/files/Ace3DS%2B_R4iLS/Ace3DS%2B_R4iLS_Wood_R4_1.62.7z) - This is from the flashcard archive's github history
1. Extract it
1. Copy the kernel files to the root of your micro SD card

Another place to download this from is r4isdhc.com.cn - though this contains a pirated GBA bios and it does not include \_DS\_MENU.dat, meaning it won't work on some carts

As mentioned before, if you want the emulators, I would suggest using Twilight Menu ++ instead as it is still maintained!

## Patching your games

There are two methods which can be used to patch your games, those are:

* Applying AP patches using the nds ROM tool
* Using a cheat database

### Applying AP patches using the nds ROM tool

You can find NDS Scene tool from here: [https://gbatemp.net/download/retrogamefan-nds-rom-tool-v1-0_b1215.35735/](https://gbatemp.net/download/retrogamefan-nds-rom-tool-v1-0_b1215.35735/). If your antivirus claims that this is malware, it's a false positive, though this seems to no longer be an issue with major AVs

To patch your rom, do the following:

1. Open the ROM tool, go into Databases>AP Database>Update Alerts then uncheck 'Enable update alerts'
1. Open the ROM in the tool by clicking the three dots, then select your rom. Or drag and drop your ROM into the tool
1. Click Export, make sure that 'Apply AP Patch' is ticked. If there is no AP patch available for your rom, this will not be an option.
1. Export your ROM!

### Using a cheat database

You can use cheats to enable AP patches without having to use the ROM tool. My go to cheat database is Deadskullzjr's cheat database: [https://gbatemp.net/threads/deadskullzjrs-nds-i-cheat-databases.488711/](https://gbatemp.net/threads/deadskullzjrs-nds-i-cheat-databases.488711/)

To set it up on this cart, follow these steps:

1. Download usrcheat.dat from the [bitbucket link](https://bitbucket.org/DeadSkullzJr/nds-i-cheat-databases/raw/963fff3858de7539891ef7918d992b8b06972a48/Cheat%20Databases/usrcheat.dat)
1. Put it into the /_rpg/cheats/ folder of your micro SD card, overwrite if prompted
1. Put the micro SD card back into the cart and launch it
1. Hover over the ROM you would like to enable the patch for. Press Y then X to enter the cheats menu
1. Hover over the AP patch and press A to enable the patch, then X to save.
1. Launch your game and enjoy!
