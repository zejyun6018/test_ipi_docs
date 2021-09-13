### How to connect Serial Console on SCDP System



By default, the EDKII is configured to use the serial console and the booting mess [HowToFlashMMCFW](HowToFlashMMCFW) ages can also be output. Before start the procedures, please prepare "U [HowToFlashMMCFW](HowToFlashMMCFW) SB to RS323 Female DB9 Serial Converter Cable" in advance.

#### **the Procedure**

- Plug the USBtoRS323 adapter cable to your host machine & SCDP system like this:

<img src="HowtoUseSerialConsole.assets/MicrosoftTeams-image.png" alt="MicrosoftTeams-image" style="zoom:67%;" />

- **In your host machine with Linux Environment:**

  -  Type this command to list the USB devices: **lsusb**

    > sushi@Sushi:~$ lsusb
    > Bus 002 Device 001: ID 1d6b:0003 Linux Foundation 3.0 root hub
    > **Bus 001 Device 011: ID 0403:6001 Future Technology Devices International, Ltd FT232 Serial (UART) IC**

  -  once detected, the devices will be under the /dev/ path to see if the interface is visible with this command: **ls /dev/ttyUSB0**

  - If you are installing a Minicom serial device then you would do the following:

    > sudo  apt-get install minicom
    >
    > sudo minicom -s

    - Go to **[Serial Port Setup] **in the Configure of minicom app
    - **Press A** and then edit to **/dev/ttyUSB0**
    - **Press E** and then edit to **115200 8N1**
    - Go to **[Exit] **

  - Then power on SCDP system and you will get the booting messages from Serial Console

     ![image-20210827154923325](HowtoUseSerialConsole.assets/image-20210827154923325.png)



- **In your Host machine with Windows Environment:** 
  - The common terminal software is putty. Putty is for free to [download](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html).
  - After execute it, please configure the following parameters:
  - Select “Connection type” to “Serial”.
  - Modify “Serial line” to the COM port which is found in the device manager.
  - Set “Speed” to **115200**.
  - Click “Open” button.

 ![windows_console](HowtoUseSerialConsole.assets/windows_console.png)