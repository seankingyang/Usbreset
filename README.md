# Usbreset
Usage:

1. Compile the program:
``` shell
$ cc usbreset.c -o usbreset
```

2. Get the Bus and Device ID of the USB device you want to reset:
```
$ lsusb  
Bus 002 Device 003: ID 0fe9:9010 DVICO  
```

3. Make our compiled program executable:
```
$ chmod +x usbreset
```

4. Execute the program with sudo privilege; make necessary substitution for <Bus> and <Device> ids as found by running the lsusb command:
```
$ sudo ./usbreset /dev/bus/usb/002/003  
```
