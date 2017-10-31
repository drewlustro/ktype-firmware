# K-Type Firmware

> Custom firmware for my K-Type. See [Configurator](https://input.club/configurator/) for GUI customization tool and load `KType-Standard.json` file.

### Layout

![ktype-v2017.0](https://i.imgur.com/I3NHUbN.jpg)

![ktype](https://user-images.githubusercontent.com/194885/32202612-575671ee-bdb4-11e7-9579-9ff60f313ae5.gif)

### Versions

| Release | &nbsp; |
| ------- | -----  |
| **[v2017.0](https://github.com/drewlustro/ktype-firmware/releases/tag/v2017.0)**   |  original release |


### Mac OSX

* Open a terminal
* May require root permissions
* **Use brew** (recommended) `brew install dfu-util`
* Enter DFU Flash Mode (e.g. press flash button), the debug led will turn on.
* **Flash** `dfu-util -D <.dfu.bin>`
* Debug led will turn off
* Keyboard is ready!

```bash
brew install dfu-util # installs dfu-util

cd whitefox-firmware  # go into correct directory

# place whitefox in "Flash Mode" via back hardware button or <CAPSLOCK>+<L-CTRL>+<ESC>
sudo dfu-util -D kiibohd.dfu.bin # uploads firmware to keyboard
```

### Linux

Unfortunately/fortunately, there are a large number of Linux distributions.
Below is the currently list of tested Linux distributions.
If you know how to successfully load firmware on another distribution, please add it here :D
In general it should be as simple as installing `dfu-util`.

* Plug in keyboard
* Open a terminal
* May require root permissions
* Install `dfu-util` package (see distro section below)
* Enter DFU Flash Mode (e.g. press flash button), the debug led will turn on.
* Flash using `dfu-util -D <.dfu.bin>`
* Debug led will turn off
* Keyboard is ready!


