# Tvheadend PVR addon for MrMC

This is a [MrMC] (http://mrmc.tv) PVR addon for connecting to a [tvheadend](https://tvheadend.org) backend.

## Build instructions

### Linux

1. `git clone https://github.com/mrmc/mrmc.git`
2. `git clone https://github.com/mrmc/pvr.hts.git`
3. `cd pvr.hts && mkdir build && cd build`
4. `cmake -DADDONS_TO_BUILD=pvr.hts -DADDON_SRC_PREFIX=../.. -DCMAKE_BUILD_TYPE=Debug -DCMAKE_INSTALL_PREFIX=../../xbmc/addons -DPACKAGE_ZIP=1 ../../xbmc/project/cmake/addons`
5. `make`

The addon files will be placed in `../../xbmc/addons` so if you build Kodi from source and run it directly 
the addon will be available as a system addon.

##### Useful links

* [MrMC's PVR user support] (http://forum.mrmc.tv)
* [MrMC's PVR development support] (http://forum.mrmc.tv)
