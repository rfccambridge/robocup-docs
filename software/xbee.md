# XBEES

Most of the xbee test scripts 


## Debugging

Most of the common problems are caused by xbee settings or file permissions. 

### USB Location

Make sure you have the right USB location. For example, make sure the current user has permissions for ```/tty/USB0``` or that the main robocup transmitter is even connected to ```USB0``` instead of ```USB1```. 

### Baud Rate

Make sure that the XBEE Baud rate is set correctly. We are currently using ```9600 [3]```, even though some of the code references ```57600 [6]```. 

### API Mode

Make sure that the API mode is set to on, [1]. You will get a -17 error if not. 




