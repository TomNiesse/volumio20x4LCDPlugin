# Welcome

Welcome to the project page for a plugin I created for Volumio2 for the Raspberry Pi.
It can retreive information about songs and webradio's and print them on an LCD-screen with I2C (4x20).<br>Pictures of the 4x20 LCD:
<img width="380px" src='https://www.raspberrypi-spy.co.uk/wp-content/uploads/2015/04/i2c_backpack_02-1024x597.jpg' alt='LCD_back'><br>
<img width="380px" src='http://domoticx.com/wp-content/uploads/YM2004A-LCD-Display-2x20-4x20.jpg' alt="LCD_front">

## How to connect the LCD

<img width="400px" src='https://i.pinimg.com/originals/84/46/ec/8446eca5728ebbfa85882e8e16af8507.png' alt='pi3_pinout'><br>
Using the image above as a reference:
  - VCC => 5V    (pin 02 or pin 04)
  - GND => GND   (There are multiple GND pins, but pin 06 is the closest)
  - SCL => SCL1  (pin 05)
  - SDA => SDA1  (pin 03)

## How to install the plugin
- Go to http://your_volumio_name.local (or http://your_volumio_ip/ if the first option does not work)
- Click the gears-icon in the top-right
- Click "PLUGINS"
- Click "Upload Plugin"
- Upload plugin.zip
- After the plugin has been successfully installed, reboot volumio<br>Optional: You can SSH into volumio and run 'sudo /etc/init.d/volumioLCDservice' instead of rebooting

## How to uninstall the plugin
The plugin can be uninstalled as any other Volumio plugin:
- Go to the installed plugins and click "Uninstall"

After uninstalling, the LCD might still show some text and it will look like it froze.<br>I will fix this in the future. It is nothing to worry about though.

## Change plugin settings

The plugin settings cannot be changed via the plugin-settings yet.<br>However, after installing the plugin, you can change '/opt/LCDcontroller/settings.py' to tweak some settings.<br>This is something that I will fix in the future

## Turning the plugin on and off

This plugin cannot be turned on or off via the plugin-settings yet. The plugin stays enabled until it is uninstalled.<br>I will fix this in the future
