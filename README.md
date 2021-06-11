# FXOSBinary
Build artifact of the FX/OS build


This repo contains the binary for testing the latest FX/OS build.  The current status of the binary is alpha quality.  The source will follow once I have stablized it.

![Screenshot 2021-06-11 10-06-41](https://user-images.githubusercontent.com/37045780/121708148-e3c54f80-ca9c-11eb-9615-5908e348c706.png)

You can poke around in the desktop, but don't expect too much yet.  Under Accessories, there is a calculator that functions (at least the first time).
I have added the API base location in the About FX/OS popup.

I have included a tools to push to the **Foenix C256**, or you can use the IDE.

```
c256serial.bat -s28 boot.hex -p XR21B1411
```

For development cross-compatibility the tool is java based, so you need at least Java 8 installed.

You can catch debug information if you hook a terminal to a COM port.  The upload tool can idintify it for you.

```
G:\>c256serial

NOTE: Ensure the debugport USB cable is connected and JTAG is NOT connected.

CURRENT ENVIRONMENT:

java Home:

java bin: java.exe

Script Directory: G:\devprojects\c256Foenix\fxos\FXOSWorkspace\FXOSv1\src\

Classpath Directory: G:\devprojects\c256Foenix\fxos\FXOSWorkspace\FXOSv1\src\serial\lib

JAR Directory: C256SerialDebugger.jar

Tools Class: com.c256.foenix.SerialTool

Port:COM1
        Desc  :Communications Port (COM1)[Serial0]
        Baud  :9600
        Data  :8
        Stop  :1
        Parity:0
        HS:0
Port:COM2
        Desc  :Communications Port (COM2)[Serial1]
        Baud  :9600
        Data  :8
        Stop  :1
        Parity:0
        HS:0
Port:COM15
        Desc  :XR21B1411 USB UART (COM15)[XR21B1411]
        Baud  :9600
        Data  :8
        Stop  :1
        Parity:0
        HS:0
Port:COM27
        Desc  :Silicon Labs CP210x USB to UART Bridge (COM27)[CP2102 USB to UART Bridge Controller]
        Baud  :9600
        Data  :8
        Stop  :1
        Parity:0
        HS:0
```

* In this case, you would be interested in this device:

```
Port:COM27
        Desc  :Silicon Labs CP210x USB to UART Bridge (COM27)[CP2102 USB to UART Bridge Controller]
```

***As always, as special thanks to Stef***
