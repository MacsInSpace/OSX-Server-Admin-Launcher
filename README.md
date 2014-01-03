OSX-Server-Admin-Launcher
=========================

OS X Server Admin Launcher (Apple Script) for 10.8 and 10.9

This launcher is a silent applescript to run Server Admin for 10.8 and 10.9 so you can manage those rock solid older servers... ;)

It requires:
--10.7.5 Server Admin
--/System/Library/PrivateFrameworks/GeoKit.framework (from 10.7.5)
--/System/Library/PrivateFrameworks/ServerKit.framework (from 10.7.5)

Where you get them is not my problem ;)

Notes:
GeoKit is in 10.8 and 10.9 but we add the packaged 10.7.5 copy to the same location via a symbolic link and move the 10.8/9 copy to "ORIGINAL" while running.
ServerKit is not in 10.8 or 10.9 so we make an symbolic link to the packaged copy.
This is all moved back once Server Admin has been Quit.
We add our local resources forder to PATH and export PATH so the system can locate the ServerKit executable.








Instructions
copy the serverkit executable from inside ServerKit.framework into the AppleScript resource folder.
copy the geokit executable from inside GeoKit.framework into the AppleScript resource folder.
copy Server Admin.app, GeoKit.framework and ServerKit.framework into the AppleScript resource folder.
