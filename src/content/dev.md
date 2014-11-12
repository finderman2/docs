---
word: Dev
title: Spark Dev
order: 6
---

Build Apps with Spark Dev
===

Introduction
===

![IDE Menu]({{assets}}/images/ide-menu.jpg)

Every command is available from **Spark** menu item. Depending on being logged in or having selected a device, this menu will change.

![Command Palette]({{assets}}/images/ide-palette.jpg)

If you prefer more keyboard oriented workflow, there's **Command Palette** with all available commands, which can be filtered.

To show the palette press `Command`, `Shift` and `P` keys together on a Mac or `Control`, `Shift`, `P` on Windows.

![Toolbar]({{assets}}/images/ide-toolbar.jpg)
**Tip**: you can change toolbar's position in settings.

There's also a toolbar on left side of IDE (it looks just like one from [Web IDE (Build)](/build) isn't it?), which contains shortcuts to most used commands like compiling or flashing.

Logging In
---
If you want to work on more advanced projects, Spark Dev could be the choice for you. Head over and download latest release:

[Spark Dev Download >](https://github.com/spark/spark-dev/releases/latest)

![IDE Window]({{assets}}/images/ide-window.jpg)

To access most of features you need to log in using your Spark account (which you can [create here](https://www.spark.io/signup)) by clicking link on the bottom of the window.

![Logging in]({{assets}}/images/ide-log-in.jpg)

Enter your email and password then click the "Log In" button. After quick verification, dialog will hide and link from the bottom will show your current account email.

**NOTE**: Using [Command Line](/cli) you'll notice that log-in status is shared between Spark Dev and CLI. So if you successfully ran `spark login`, you will be logged in within the Spark Dev.

Selecting device
---

![Selecting device]({{assets}}/images/ide-select-core.jpg)

Most of features like **Flashing** or accessing **Cloud variables and functions** requires selecting which device they will interact with.

There are three ways to select core:

* Click **Select device** button in the left toolbar
* Click device's name on the bottom of the window
* Click on **Spark** -> **Select device...** menu

Then you will see list of all your device along with online indicator. You can search for specific one by typing its name. Clicking on device or pressing `Enter` when device is selected, will make it the current one.

Compiling code
---

![Compile button]({{assets}}/images/ide-compile.jpg)

To compile your current project, click on the **Compile in the cloud** button. If your code doesn't contain errors, you'll see a new file named **firmware_X.bin** in your project's directory (where *X* is a timestamp).

![Compile errors]({{assets}}/images/ide-compile-errors.jpg)

If there are some errors, you'll see a list of them allowing you to quickly jump to relevant line in code. You can show this list by clicking red error icon on the bottom of the window.

Flashing device
---

![Flash button]({{assets}}/images/ide-flash.jpg)

When you're sure that your code is correct it's time to flash it to the device. To do this, click **Flash using cloud** button. Your code will be sent wirelessly to your device. If the flash was successful, the LED on your device will begin flashing magenta.

Cloud variables & functions
===

To access all registered variables and functions, go to **Spark** -> **Show cloud variables and functions** menu.

Variables
---

![Getting variable]({{assets}}/images/ide-get-variable.gif)

All registered variables are shown on the left side of panel. To get lastest variable value, click **Refresh** button for variable you want to update.

![Watching variable]({{assets}}/images/ide-watch-variable.gif)

When you want to check variable value constantly, you can start watching it by clicking **Watch** button. When variable is watched, Spark Dev will fetch latest value every 5 seconds.

Functions
---

![Functions]({{assets}}/images/ide-functions.gif)

To call a function, just click on the button with its name. After finishing you'll see its result on the right side.

You can also add parameters to the call by entering them on the right of button.

Managing device
===

Using Spark Dev you can do many things with your device including setting up its WiFi, claiming or renaming it.

Setting up WiFi
---

![WiFi list]({{assets}}/images/ide-wifi-list.jpg)

To setup device's WiFi, connect it via USB and click **Setup device's WiFi...** button on the toolbar.

If your device isn't in [listening mode](/connect/#connecting-your-core-listening-mode) you'll see animation showing how to enter it.

Next you'll see all available networks. One you are currently connected to will be first.

Select one you want device to use or choose **Enter SSID manually** (last item) to specify all information by hand.

![WiFi setup]({{assets}}/images/ide-wifi-save.jpg)

Now you need to fill missing information and click **Save**. Core will go dark for a second and then try to connect to the WiFi.