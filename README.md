# SimpleHTTPr
Serves a default.htm .gif .jpg .swf or .js file from it's \wwwroot directory and can also run batch files locally.

Tested on Windows XP, Server 2003, Vista, Server 2008, Windows 7, Windows 8, Windows 10, Windows 11

A scripted install/uninstall is not included with this software.

This program runs as a service; without any GUI, taskbar, or system tray icon.

## Installation

1) Ensure the Microsoft .NET Framework 4.x is installed
2) Right-click on the .zip file you downloaded, select properties, click the Unblock button (if this button is not present just proceed)
3) Extract the contents of the .zip file (usually to C:\SimpleHTTP)
4) Edit SimpleHTTPr.ini to include the IP of your server and path to the default.x files (usually C:\SimpleHTTP\wwwroot)
5) Right-click on _setup_.bat and select "Run as administrator" to install the service (see note at bottom of this text)

Anytime you make a change in SimpleHTTP.ini you must restart the service for it to take effect.

## Usage

SimpleHTTPr v3.0.0.3 will also serve the following files when requested and found in the path...

- /default001.htm through /default005.htm
- /default001.gif through /default005.gif
- /default001.jpg through /default005.jpg
- /default001.swf through /default005.swf
- /run001.htm through /run005.htm, when requested, will start the matching run001.bat through run005.bat on the server

Alternatively, SimpleHTTPrm v3.0.0.7 (Run More) will serve files /default001.* through /default030.* and /run001.* through /run0030.*

No GUI is displayed, check Task Manager or tcpview to see that it's running.

Note: Under Windows Vista and later OS versions you may receive an error (HRESULT: 0x80131515) when installing the service.
The solution is to save the .zip file, right-click on it, select properties, and click the Unblock button.
Then extract the contents of the .zip file. Right-click on _setup_.bat and select "Run as administrator" and it will work.

## License

GPL does not allow you to link GPL-licensed components with other proprietary software (unless you publish as GPL too).

GPL does not allow you to modify the GPL code and make the changes proprietary, so you cannot use GPL code in your non-GPL projects.

If you wish to integrate this software into your commercial software package, or you are a corporate entity with more than 10 employees, then you should obtain a per-instance license, or a site-wide license, from http://jpelectron.com/buy

For all other use cases please consider: <a href='https://ko-fi.com/C0C54S4JF' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://cdn.ko-fi.com/cdn/kofi2.png?v=2' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>

[End of Line]
