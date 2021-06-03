# FXOSBinary
Build artifact of the FX/OS build


This repo contains the binary for testing the latest FX/OS build.  The current status of the binary is alpha qaulity.  The source will follow once I have stablized it.


You can poke around in the desktop, but don't expect too much yet.  Under Accessories, there is a calculator that functions (at least the first time).


I have included a tools to push to the Foeix, or you can use the IDE.

```
c256serial.bat -s28 boot.hex -p XR21B1411
```

For development cross-compatibility the tool is java based, so you need at least Java 8 installed.
