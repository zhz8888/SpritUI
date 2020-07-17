# SpritUI

![SpritUI](https://s1.ax1x.com/2020/07/17/UsWFGn.png)

> If you are tired with flashing Native Android, try SpritUI.

SpritUI is a High-Customize UI Android Project, based on AospExtended.

## Credits
* [**AospExtended**](https://github.com/AospExtended)
* [**JDCTeam**](https://github.com/AOSP-JF-MM)
* [**DirtyUnicorns**](https://github.com/DirtyUnicorns)
* [**TeamSubstratum (Theme Engine)**](https://github.com/Substratum)
* [**LineageOS/Cyanogenmod**](https://github.com/LineageOS)
* [**Nitrogen Project**](https://github.com/nitrogen-project)
* [**ABC ROM**](https://github.com/ezio84)
* [**GZOSP**](https://github.com/GZOSP)
* [**Pure Nexus**](https://github.com/PureNexusProject)
* [**OmniROM**](https://github.com/omnirom/)
* [**AOSPA**](https://github.com/aospa/)
* [**BlissRoms**](https://github.com/BlissRoms)

## How to Build?

To initialize your local repository using the SpritUI trees, use a 
command like this:

```bash
  repo init -u git://github.com/SpritHub/manifest.git -b 10.x
```
To initialize a shallow clone, which will save even more space & time, use a command like this:

```bash
  repo init --depth=1 -u git://github.com/SpritHub/manifest.git -b 10.x
```
  
### Then to sync up:

```bash
  repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```
### Finally to build:

```bash
  . build/envsetup.sh
  lunch aosp_{device_codename}-userdebug
  mka aex -j$(nproc --all) | tee log.txt
```
