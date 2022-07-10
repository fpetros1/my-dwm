# Self-Patched DWM
Created a new build of DWM to learn and experience the philosophy of Suckless software

# Patches
- 01 - [![AutoStart](https://img.shields.io/badge/DWM-AutoStart-blue)](https://dwm.suckless.org/patches/autostart/)
- 02 - [![Status2d-Systray](https://img.shields.io/badge/DWM-Status2D(With%20System%20Tray)-blue)](https://dwm.suckless.org/patches/status2d/)
- 03 - [![Attach-Bottom](https://img.shields.io/badge/DWM-Attach%20Bottom-blue)](https://dwm.suckless.org/patches/attachbottom/)
- 04 - [![Always-Center](https://img.shields.io/badge/DWM-Always%20Center-blue)](https://dwm.suckless.org/patches/alwayscenter/)
- 05 - [![Float-Rules](https://img.shields.io/badge/DWM-Float%20Rules-blue)](https://dwm.suckless.org/patches/floatrules/)
- 06 - [![Per-Tag](https://img.shields.io/badge/DWM-Per%20Tag-blue)](https://dwm.suckless.org/patches/pertag/)
- 07 - [![Centered-Master](https://img.shields.io/badge/DWM-Centered%20Master-blue)](https://dwm.suckless.org/patches/centeredmaster/)
- 08 - [![Cycle-Layouts](https://img.shields.io/badge/DWM-Cycle%20Layouts-blue)](https://dwm.suckless.org/patches/centeredmaster/)
- 09 - [![Vanity-Gaps](https://img.shields.io/badge/DWM-Vanity%20Gaps-blue)](https://dwm.suckless.org/patches/vanitygaps/)
- 10 - [![Scratchpads](https://img.shields.io/badge/DWM-Scratchpads-blue)](https://dwm.suckless.org/patches/scratchpads/)

# Requirements
- Alacritty
- dmenu
- Bitwarden (bitwarden-desktop on $PATH)

# Extensions
- [![slstatus](https://img.shields.io/badge/fpetros1-Custom%20slstatus-blue)](https://github.com/fpetros1/my-slstatus/)

# Post-Install
- Create a script named either "autostart.sh"(for non-blocking scripts) or "autostart-blocking.sh"(for blocking scripts) in $XDG_DATA_HOME/dwm, if $XDG_DATA_HOME is not set, then: "$HOME/.local/share/dwm". Ex: `echo -e '#!/bin/sh\n' > $XDG_DATA_HOME/dwm/autostart.sh`
- Add slstatus(if installed) to autostart. Ex: `echo -e 'slstatus &\n' >> ./autostart.sh`
- Make script(s) executable. Ex: `chmod +x $XDG_DATA_HOME/dwm/autostart.sh`
- Restart DWM

# Important Keybindings

### NOTE: `Mod` = `Super/Windows` Key

### Spawn Commands
| Keys                            | Action                 |
|---------------------------------|------------------------|
| `Mod`+`Enter`                   | Alacritty              |
| `Mod`+`Shift` `b`               | Bitwarden(Scratchpad)  |
| `Mod`+`p`                       | rofi                   |

### Tag Commands
| Keys                      | Action                     |
|---------------------------|----------------------------|
| `Mod`+`{1 ... 9}`         | Change to Tag {1 ... 9}    | 
| `Mod`+`Shift`+`{1 ... 9}`| Send focused window to tag |

### Layout Commands
| Keys                                                      | Action                                            |
|-----------------------------------------------------------|---------------------------------------------------|
| `Mod`+`Shift`+`Enter`                                     | Send focused window to the top of the stack       |
| `Mod`+`Ctrl`+`.` (next) OR `Mod`+`Ctrl`+`.` (previous)    | Cycle Layouts                                     |
| `Mod`+`j` (next) OR `Mod`+`k` (previous)                  | Move focus between windows                        |
| `Mod`+`h` (increase) OR `Mod`+`l` (decrease)              | Manipulate window on top of the stack (master)    |

### Window Commands
| Keys                                              | Action                         |
|---------------------------------------------------|--------------------------------|
| `Mod`+`q`                                         | Kill focused window            |
| `Mod`+`Shift`+`Space`                             | Make focused window float      |
| `Mod`+`Shift`+`Middle Mouse Button`               | Make focused window un-float   |

### Session Commands
| Keys                            | Action                 |
|---------------------------------|------------------------|
| `Mod`+`Shift`+`q`               | Quit DWM cleanly       |

# Original README
[![original-README](https://img.shields.io/badge/README-Suckless-blue)](SUCKLESS.README)
