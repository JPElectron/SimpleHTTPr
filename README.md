# SimpleHTTPr
Serves a default.htm .gif .jpg .swf or .js file from it's \wwwroot directory and can also run batch files locally.

Tested on Windows XP, Server 2003, Vista, Server 2008, Windows 7, Windows 8

A scripted install/uninstall is not included with this software.

This program runs as a service; without any GUI, taskbar, or system tray icon.

<b>Installation:</b>

1) Ensure the Microsoft .NET Framework 4.x is installed
2) Right-click on the .zip file you downloaded, select properties, click the Unblock button (if this button is not present just proceed)
3) Extract the contents of the .zip file (usually to C:\SimpleHTTP)
4) Edit SimpleHTTPr.ini to include the IP of your server and path to the default.x files (usually C:\SimpleHTTP\wwwroot)
5) Right-click on _setup_.bat and select "Run as administrator" to install the service (see note at bottom of this text)

Anytime you make a change in SimpleHTTP.ini you must restart the service for it to take effect.

<b>Usage:</b>

SimpleHTTPr will also serve the following files when requested and found in the path...

- /default001.htm through /default005.htm
- /default001.gif through /default005.gif
- /default001.jpg through /default005.jpg
- /default001.swf through /default005.swf
- /run001.htm through /run005.htm, when requested, will start the matching run001.bat through run005.bat on the server

No GUI is displayed, check Task Manager or tcpview to see that it's running.

Note: Under Windows Vista and later OS versions you may receive an error (HRESULT: 0x80131515) when installing the service.
The solution is to save the .zip file, right-click on it, select properties, and click the Unblock button.
Then extract the contents of the .zip file. Right-click on _setup_.bat and select "Run as administrator" and it will work.
