### My Battery Max is simple program that tells you when you should unplug or plug your laptop charger :octocat:
_this program need acpi to working properly_

#### to use MyBattMax
* install acpi and gtk3 `sudo apt install acpi gtk+-3.0 -y`
* clone this repo
* goto GUI directory
* `make`
* add `mybatmax` to startup
* and you're done!

#### to use AnimeInterface
* clone telegram library <https://github.com/tdlib/td>
* install tdlib depedency <https://github.com/tdlib/td#dependencies>
* compile telegram library _"assuming library will go to home `~/tdlib`"_
```bash
cd <path to TDLib sources>
mkdir build
cd build
cmake -DCMAKE_BUILD_TYPE=Release -DCMAKE_INSTALL_PREFIX:PATH="~/tdlib" ..
cmake --build . --target install
```
* then compile aiface
```bash
cd <path to MyBattMax sources>/AnimeInterface
mkdir build
cd build
cmake -DCMAKE_BUILD_TYPE=Release -DTd_DIR="~/tdlib/lib/cmake/Td" ..
cmake --build .
```
* Aiface is under progress!

_some image copyright goes to the respective owner_

_personal use only!_
