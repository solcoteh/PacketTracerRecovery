# PacketTracer - Password Cracker Tool
This tool is build for PacketTracer, and its goal is to perform password recovery on any given 'Activity File' or '.pka' file.
The tool simply hooks the password function inside PacketTracer, and replaces the original hash with the following one: ``805F4011727E7FA3FC5D7FFEE2BBB5EC``.
After that user needs to use "Ferib" as password and can now gain access to the 'Activity Wizard'. From there you can change the password to whatever you'd like.

```bash
sudo apt install mono-devel mono-xbuild

└─$ git clone https://github.com/solcoteh/PacketTracerRecovery
cd PacketTracerRecovery && xbuild PacketTracerPatcher.csproj
# copy ./bin/Debug/PacketTracerPatcher.exe with Winscp to Windows  
```

# TL;TR
This tool changes the PacketTracer password to "Ferib".
You can then change the password to whatever you like in the 'Activity Wizard'.

# Video Showcase
![gif](https://github.com/ferib/PacketTracerRecovery/blob/master/img/showcase.gif?raw=true)

# How To
* Start PacketTracer7
* Open your .pka
* Start PacketTracerPatcher.exe
* Go to PacketTracer7 and navigate to Extensions -> Activity Wizard (or press ctrl+w)
* Enter 'Ferib' as password
* Select Password in the left navigation
* Enter new password and click Enable Password

*Password has now been changed, in order to save the changes, click on Save or Save As*

# Disclaimer
Please use at your own risk.

