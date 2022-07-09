# Self-Patched DWM
Created a new build of DWM to learn and experience the philosophy of Suckless software

# Patches
- [![AutoStart](https://img.shields.io/badge/DWM-AutoStart-blue)](https://dwm.suckless.org/patches/autostart/)
- [![Status2d-Systray](https://img.shields.io/badge/DWM-Status2D(With%20System%20Tray)-blue)](https://dwm.suckless.org/patches/status2d/)
- [![Attach-Bottom](https://img.shields.io/badge/DWM-Attach%20Bottom-blue)](https://dwm.suckless.org/patches/attachbottom/)
- [![Always-Center](https://img.shields.io/badge/DWM-Always%20Center-blue)](https://dwm.suckless.org/patches/alwayscenter/)
- [![Always-Center](https://img.shields.io/badge/DWM-Always%20Center-blue)](https://dwm.suckless.org/patches/alwayscenter/)
- [![Float-Rules](https://img.shields.io/badge/DWM-Float%20Rules-blue)](https://dwm.suckless.org/patches/floatrules/)
- [![Per-Tag](https://img.shields.io/badge/DWM-Per%20Tag-blue)](https://dwm.suckless.org/patches/pertag/)
- [![Centered-Master](https://img.shields.io/badge/DWM-Centered%20Master-blue)](https://dwm.suckless.org/patches/centeredmaster/)
- [![Cycle-Layouts](https://img.shields.io/badge/DWM-Cycle%20Layouts-blue)](https://dwm.suckless.org/patches/centeredmaster/)
- [![Vanity-Gaps](https://img.shields.io/badge/DWM-Vanity%20Gaps-blue)](https://dwm.suckless.org/patches/vanitygaps/)
- [![Scratchpads](https://img.shields.io/badge/DWM-Scratchpads-blue)](https://dwm.suckless.org/patches/scratchpads/)

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

### NOTE: `MOD` = `Super/Windows` Key

### Spawn Commands
| Keys                            | Action                 |
|---------------------------------|------------------------|
| `MOD` `Shift` `Enter`           | Alacritty              |
| `MOD` `Shift` `b`               | Bitwarden(Scratchpad)  |
| `MOD` `p`                       | dmenu                  |

### Layout Commands
| Keys                                                      | Action                                            |
|-----------------------------------------------------------|---------------------------------------------------|
| `MOD` `Enter`                                             | Send focused window to the top of the stack       |
| `MOD` `Ctrl` `.` (next) OR `MOD` `Ctrl` `.` (previous)    | Cycle Layouts                                     |
| `MOD` `j` (next) OR `MOD` `k` (previous)                  | Move focus between windows                        |
| `MOD` `h` (increase) OR `MOD` `l` (decrease)              | Manipulate window on top of the stack (master)    |

### Window Commands
| Keys                                              | Action                 |
|---------------------------------------------------|------------------------|
| `MOD` `Shift` `c`                                 | Kill focused window    |
| `MOD` `Shift` `Space`                             | Make window float      |
| `MOD` `Shift` `Middle Mouse Button`               | Make window un-float   |

### Session Commands
| Keys                            | Action                 |
|---------------------------------|------------------------|
| `MOD` `Shift` `q`               | quit DWM cleanly       |

# Original README
[![original-README](https://img.shields.io/badge/README-Suckless-blue)](SUCKLESS.README)
