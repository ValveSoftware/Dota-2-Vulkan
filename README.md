# Dota-2-Vulkan
Tracker for issues specific to the Vulkan version of Dota 2 on Windows and Linux

Notes:

* This tracker is only for issues impacting the Vulkan version of Dota 2.  For non-Vulkan Dota 2 Linux/OS X issues please use https://github.com/ValveSoftware/Dota-2.  For all other Dota 2 bugs, use http://dev.dota2.com/.
* Before filing a bug, please make sure your system meets the minimum requirements and you have a supported driver installed.
* Please make sure to opt-in to the Steam Client Beta for the latest Steam Vulkan Overlay (fixes performance issue with Steam Overlay) 
* Enable with the -vulkan launch option after downloading the Vulkan Beta DLC.  Remove -dx9/-dx11/-gl (if present) from any previous launch options. You will know if you're properly running Vulkan if Vulkan-specific commands are available in the console, such as 'vulkan_memgr_print'
* Minimum requirements for Dota 2 Vulkan:
 * Windows 7/8/10 64-bit: NVIDIA Kepler-series+ (365.19+ driver), AMD 7700+ (Crimson 16.5.2.1+ driver)
   * NOTE: NVIDIA __Fermi GPUs are not supported__, this includes some models in the 600/700/800 series, so please make sure you have a Kepler (GKxxx), Maxwell (GMxxx), or Pascal (GPxxx) GPU before posting a bug.  This is especially confusing because some models such as the GT730 have both a Fermi and Kepler model.  You can check for sure by looking up your [NVIDIA PCI Device ID] (https://pci-ids.ucw.cz/read/PC/10de).  The Device ID can be found in Steam -> Help -> System Information.
 * Linux 64-bit: NVIDIA 600-series+ (364.16+ driver), AMD GCN 1.2 (16.20.3 driver)
 * 2GB of GPU Memory required - may experience crashes with < 2GB of GPU memory.
 * Vulkan is not supported on Mac OS X.

If the game fails to launch with a "missing executable" error, please use Steam to [verify the integrity](https://support.steampowered.com/kb_article.php?ref=2037-QEUH-3335) of the game's files in order to acquire the missing binaries.

Known Issues
------------

* The first time you run with Vulkan you may experience short stutters while the engine caches shaders on disk. After playing through or watching a match, these stutters should go away.
*     There is a known issue on Linux with NVIDIA GPUs where tearing can be observed even when vertical sync is enabled. NVIDIA is aware of the issue and it will be fixed in the future through a driver update.

Conduct
-------

There are basic rules of conduct that should be followed at all times by everyone participating in the discussions.  While this is generally a relaxed environment, please remember the following:

- Do not insult, harass, or demean anyone.
- Do not intentionally multi-post an issue.
- Do not use ALL CAPS when creating an issue report.
- Do not repeatedly update an open issue remarking that the issue persists.

Remember: Just because the issue you reported was reported here does not mean that it is an issue with Dota 2 Reborn.  As well, should your issue not be resolved immediately, it does not mean that a resolution is not being researched or tested.  Patience is always appreciated.

Reporting Issues
----------------

If you encounter a bug while using Dota 2 Vulkan, first search the [issue list](https://github.com/ValveSoftware/Dota-2-Vulkan/issues) to see if it has already been reported. Include closed issues in your search.

If it has not been reported, create a new issue with at least the following information:

- what platform this is occurring  on: Linux or Windows 7/8/10;
- a short, descriptive title;
- a detailed description of the issue, including any output from the command line;
- steps for reproducing the issue; and
- your [system information](#system-information).

Please place logs either in a code block (press `M` in your browser for a GFM cheat sheet) or a [gist](https://gist.github.com).

### System information

Your system information must include:
- your Linux distro or Windows version
- if Linux, your Desktop/Window Manager
- your Graphics card info (manufacturer, card version), any and all graphics driver versions
- anything else that you think may be useful (mouse/keyboard, filesystem type, etc).

The preferred and easiest way to get this information is from Steam's Hardware Information viewer from the menu (`Help -> System Information`).

Once your information appears: right-click within the dialog, choose `Select All`, right-click again, and then choose `Copy`.
Paste this information into your report, preferably in a code block or a [gist](https://gist.github.com).

Feature Requests
-------------------

This repository is not meant for Dota 2 feature requests. There are forums dedicated to general Dota 2 discussion at http://dev.dota2.com.

