OSX-Server-Admin-Launcher
=========================

OS X Server Admin Launcher (Apple Script) for 10.8 and 10.9<BR>

This launcher is a silent applescript to run Server Admin for 10.8 and 10.9 so you can manage those rock solid older<BR> servers... ;)<BR>

It requires:<BR>
--10.7.5 Server Admin<BR>
--/System/Library/PrivateFrameworks/GeoKit.framework (from 10.7.5)<BR>
--/System/Library/PrivateFrameworks/ServerKit.framework (from 10.7.5)<BR>
<BR>
Where you get them is not my problem ;)<BR>
<BR>
Notes:<BR>
GeoKit is in 10.8 and 10.9 but we add the packaged 10.7.5 copy<BR> 
to the same location via a symbolic link and move the 10.8/9 copy to "ORIGINAL" while running.<BR>
ServerKit is not in 10.8 or 10.9 so we make an symbolic link to the packaged copy.<BR>
This is all moved back once Server Admin has been Quit.<BR>
We add our local resources forder to PATH and export PATH so the system can locate the ServerKit executable.<BR>








Instructions:<BR>
Create a new Applescript Application bundle:
<a href="http://imgur.com/0nNL2aZ"><img src="http://i.imgur.com/0nNL2aZ.png" title="Hosted by imgur.com"/></a><BR>
copy the serverkit executable from inside ServerKit.framework into the AppleScript resource folder.<BR>
copy the geokit executable from inside GeoKit.framework into the AppleScript resource folder.<BR>
copy Server Admin.app, GeoKit.framework and ServerKit.framework into the AppleScript resource folder.<BR>
<a href="http://imgur.com/smueIzo"><img src="http://i.imgur.com/smueIzo.png" title="Hosted by imgur.com"/></a><BR>

<BR>
Edit the AppleScripts Info.plist and add:<BR>
<key>LSBackgroundOnly</key><BR>
<string>1</string><BR>
<a href="http://imgur.com/0nNL2aZ"><img src="http://i.imgur.com/0nNL2aZ.png" title="Hosted by imgur.com"/></a><BR>

<a href="http://imgur.com/MG2sT4E"><img src="http://i.imgur.com/MG2sT4E.png" title="Hosted by imgur.com"/></a><BR>
