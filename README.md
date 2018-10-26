# xorg-fix-your-shit
## tearfree xorg configs
here so I don't lose it

---

### /etc/X11/xorg.conf.d/20-intel.conf
```
Section "Device"
    Identifier    "Intel Graphics"
    Driver        "intel"
    Option        "AccelMethod"        "sna"
    Option        "TearFree"        "true"
EndSection
```
### /etc/X11/xorg.conf.d/20-amdgpu.conf
```
Section "Device"
    Identifier "AMD"
    Driver "amdgpu"
    Option "TearFree" "true"
EndSection
```
### /etc/X11/xorg.conf.d/20-radeon.conf
```
Section "Device"
    Identifier "Radeon"
    Driver "radeon"
    Option "TearFree" "on"
EndSection
```
