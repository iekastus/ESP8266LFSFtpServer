# esp8266LFSFTPServer
Simple FTP Server for using esp8266/esp32 SPIFFs

Now should support esp32!!!  

I've modified a FTP server from arduino/wifi shield to work with esp8266....

This allows you to FTP into your esp8266 and access/modify the LittleFS folder/data...it only allows one ftp connection at a time....very simple for now...

I've tested it with Filezilla, and the basics work (upload/download/rename/delete). There's create/modify directory support.

You need to setup Filezilla(or other client) to only allow 1 connection..
To force FileZilla to use the primary connection for data transfers:
Go to File/Site Manager then select your site.
In Transfer Settings, check "Limit number of simultaneous connections" and set the maximum to 1

only supports Passive ftp mode....

It does NOT support any encryption, so you'll have to disable any form of encryption...

feel free to try it out (sample provided)....unzip into your arduino library directory (and restart arduino ide).


this is the original project on github I worked from: https://github.com/gallegojm/Arduino-Ftp-Server/tree/master/FtpServer
