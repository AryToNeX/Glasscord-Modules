# Discord Titlebar
### Developed by [Zack senpai](https://github.com/rauenzi), maintained by [Naomi](https://github.com/AryToNeX)

**Note:** This module was formerly integrated into Glasscord <= 0.0.7.1.

## Available properties

### `--glasscord-titlebar`
#### accepts a value between those ones: `native`, `windows`, `linux`, `osx`; defaults to `native`
Changes Discord's titlebar to the one specified.
- `native` is the default one for your platform.
- `windows` is the Windows-style titlebar (buttons on the right side, full titlebar)
- `osx` is the macOS-style hidden titlebar with the minimal semaphore-style window buttons on the left.
- `linux` is the Linux-style Discord titlebar, aka the native one of your system.
Linux didn't get any of the fancy titlebars Discord has, which is sad.

**Note:** for this setting to work, you should restart Discord after loading your custom CSS!
But don't worry, this module will remind you of that.
