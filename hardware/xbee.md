# XBEE Remote Documentation


## Installing XTCU

Install XTCU and follow all of the settings. Make sure that your user has access to ```dialout``` and has permissions to access USBs since you will need root access to use the XBEE API.

Installing XTCU into your home directory ```~/``` will make your life easier. On the Robocup computers, there should be an alias
```
alias xtcu="sudo sh ~/XCTU-NG/launcher"
```

## Installing C++/XBEE Library

We are currently using [libxbee](https://github.com/attie/libxbee3), an xbee library for C/C++. The library files should already be inside ```common/include``` in the robocup-software repository, but just in case you can get the source code from the libxbee library github. 


## Manual Control XBEE

The Manual Control XBEE is the one with API MODE OFF and with the name RobocupHumanCommand. Used to connect with XTCU in console mode so you can send ASCII easily to other xbees. Mainly used for wasd controls. 

## Currently Used XBEE Settings

### RobocupMaster

* CH - F
* ID - 4200
* ICE - Coordinator [1]
* IA2 - 000b
* INI - RobocupCommand
* IBD - 57600 [6]
* IAP - API enabled [1]

### RobocupSlave01

* ICH - F
* IID - 4200
* ICE - End Device [0] 
* IA2 - 000b
* INI - RobocupSlave01
* IBD - 9600 [3]
* IAP - API enabled [1]



