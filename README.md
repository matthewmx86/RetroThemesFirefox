# RetroThemesFirefox
<h2>A collection of old browser themes for Firefox.</h2>


![Image Screenshot](https://github.com/matthewmx86/RetroThemesFirefox/blob/main/Screenshots/netscape1.png)


To install a theme, place the "chrome" directory from the theme into your Firefox user profile directory. 
Set toolkit.legacyUserProfileCustomizations.stylesheets to True in about:config and make sure to close all 
running instances of Firefox for the changes to take effect.
<br>
## About
The RetroThemesFirefox project is a collection of Firefox themes mimicking classic browsers such as Internet Explorer and Netscape.
This project is a spin off of my previous Redmond-Firefox repo with updated compatibility for the latest Firefox releases.


## Requirements
#### Main theme
The following are required:
```
firefox
```

## Limitations
Inherit color support is not currently finished.
Also the theme was designed with a certain color scheme in mind so it may not display correctly
with certain color schemes. I'm working on adding inherit functions to the theme and I'm currently 
designing a script to apply selected colors from the active GTK theme and apply it to the Firefox theme. 
For now I recommend using my default [Redmond97](https://github.com/matthewmx86/Redmond97) theme.

## Installation

Clone the repository by the following command:

```
git clone https://github.com/matthewmx86/RetroThemesFirefox.git
```
Alternatively you can download the .zip archive of the repo.

To install, you will first need to find your firefox user profile directory. It is usually the one that ends with ".default".
To find the correct directory, open a terminal and go to the hidden Firefox directory. Using grep you can view the directories
ending with ".default".
```
cd ~/.mozilla/firefox
ls | grep default
```
In this exmaple I have two directories: one .default and the other .default-release. 
![Image Screenshot](https://github.com/matthewmx86/Redmond97/blob/master/Screenshots/console.png)
If you only have one directory ending with .default that one is the correct profile directory and you can skip
this next step. Otherwise, you can run the following to see which profile is the default.
```
firefox -P
```
You will then see the following window:

![Image Screenshot](https://github.com/matthewmx86/Redmond97/blob/master/Screenshots/firefox.png)

The selected profile is your default profile, in my case it is the default-release profile.

Once you have found the correct profile directory, you can copy the chrome folder from any of the included themes 
into your Firefox profile directory. Again, using my example above, to install the Netscape theme
the command would be:
```
cp -aR ~/RetroThemesFirefox/Netscape/Netscape4/* ~/.mozilla/firefox/vugvl4ul.default-release/chrome/
```
Or you can use your file manager to copy the chrome directory into your Firefox profile directory.

Note:
[ If you have not enabled custom user style sheets (userchrome): ]
1. Navigate to "about:config" in Firefox
2. Enter the following text in the search box: toolkit.legacyUserProfileCustomizations.stylesheets
3. Set the option toolkit.legacyUserProfileCustomizations.stylesheets to True
4. Close all instances of Firefox and the changes will take effect when you restart Firefox

The Firefox theme should now be installed and will be activated once you close all Firefox sessions and restart Firefox.
<br><br>
Addons:<br>
To get the themed scrollbars in Netscape4_alt, you will need to install an autoconfig script such as the one from autoloader-fx. This will allow theming of web content widgets. The repo can be found here: https://github.com/MrOtherGuy/fx-autoconfig. Note that this is conisdered a security risk as any malicious javascript can be loaded on Firefox startup. I would recommend changing the permissions of the chrome/JS folder to readonly after installing to mitigate this issue.<br><br>

##Screenshots<br>
IE5:<br>
![Image Screenshot](https://github.com/matthewmx86/RetroThemesFirefox/blob/main/Screenshots/ie5.png)<br>
IE6:<br>
![Image Screenshot](https://github.com/matthewmx86/RetroThemesFirefox/blob/main/Screenshots/ie6.png)<br>
IE7:<br>
![Image Screenshot](https://github.com/matthewmx86/RetroThemesFirefox/blob/main/Screenshots/ie7.png)<br>
IE8:<br>
![Image Screenshot](https://github.com/matthewmx86/RetroThemesFirefox/blob/main/Screenshots/ie8.png)<br>
Netscape4:<br>
![Image Screenshot](https://github.com/matthewmx86/RetroThemesFirefox/blob/main/Screenshots/netscape.png)<br>
Netscape4_alt<br>
![Image Screenshot](https://github.com/matthewmx86/RetroThemesFirefox/blob/main/Screenshots/netscape4_alt.png)
![Image Screenshot](https://github.com/matthewmx86/RetroThemesFirefox/blob/main/Screenshots/netscape2.png)

