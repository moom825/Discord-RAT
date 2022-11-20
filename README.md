# DiscordRAT
Discord Remote Administration Tool fully written in Python3.

This is a RAT controlled over Discord with over 50 post exploitation modules.

Please use the 2.0 version\
https://github.com/moom825/Discord-RAT-2.0
## **Disclaimer:**

This tool is for educational use only, the author will not be held responsible for any misuse of this tool.

## **Credits**
This project was originally made by https://github.com/Sp00p64/DiscordRAT, this entire readme.md is made by him too.\
Credit goes to him for all the original modules and readme.md

## **Setup Guide:**
You will first need to register a bot with the Discord developer portal and then add the bot to the Discord server that you want to use to control the bot (make sure the bot has administrator privileges in the Discord server).
Once the bot is created copy the token of your bot and paste it at line 20.

Install requirements :
```
pip3 install -r requirements.txt
```
Then if the steps above were successful, you can launch the python file by executing ```python DiscordRAT.py```. It will create a new channel and post a message on the server with a generated session number.\
Now your bot should be available to use ! 

**Requirements:**\
Python3, Windows(x64)

## **Modules**
```
Available commands are :
--> !message = Show a message box displaying your text / Syntax  = "!message example"
--> !shell = Execute a shell command /Syntax  = "!shell whoami"
--> !webcampic = Take a picture from the webcam
--> !windowstart = Start logging current user window (logging is shown in the bot activity)
--> !windowstop = Stop logging current user window 
--> !voice = Make a voice say outloud a custom sentence / Syntax = "!voice test"
--> !admincheck = Check if program has admin privileges
--> !sysinfo = Gives info about infected computer
--> !history = Get chrome browser history
--> !download = Download a file from infected computer
--> !upload = Upload file to infected computer / Syntax = "!upload file.png" (with attachment)
--> !cd = Changes directory
--> !delete = deletes a file / Syntax = "!delete /path to/the/file.txt"
--> !write = Type your desired sentence on computer / Type "enter" to press the enter button on the computer
--> !wallpaper = Change infected computer wallpaper / Syntax = "!wallpaper" (with attachment)
--> !clipboard = Retrieve infected computer clipboard content
--> !geolocate = Geolocate computer using latitude and longitude of the ip adress with google map / Warning : Geolocating IP adresses is not very precise
--> !startkeylogger = Starts a keylogger
--> !stopkeylogger = Stops keylogger
--> !dumpkeylogger = Dumps the keylog
--> !volumemax = Put volume to max
--> !volumezero = Put volume at 0
--> !idletime = Get the idle time of user's on target computer
--> !blockinput = Blocks user's keyboard and mouse / Warning : Admin rights are required
--> !unblockinput = Unblocks user's keyboard and mouse / Warning : Admin rights are required
--> !screenshot = Get the screenshot of the user's current screen
--> !exit = Exit program
--> !kill = Kill a session or all sessions / Syntax = "!kill session-3" or "!kill all"
--> !uacbypass = attempt to bypass uac to gain admin by using fod helper
--> !passwords = grab all chrome passwords
--> !streamwebcam = streams webcam by sending multiple pictures
--> !stopwebcam = stop webcam stream
--> !getdiscordinfo = get discord token,email,phone number,etc
--> !streamscreen = stream screen by sending multiple pictures
--> !stopscreen = stop screen stream
--> !shutdown = shutdown computer
--> !restart = restart computer
--> !logoff = log off current user
--> !bluescreen = BlueScreen PC
--> !displaydir = display all items in current dir
--> !currentdir = display the current dir
--> !dateandtime = display system date and time
--> !prockill = kill a process by name / syntax = "!kill process.exe"
--> !recscreen = record screen for certain amount of time / syntax = "!recscreen 10"
--> !reccam = record camera for certain amount of time / syntax = "!reccam 10"
--> !recaudio = record audio for certain amount of time / syntax = "!recaudio 10"
--> !disableantivirus = permanently disable windows defender(requires admin)
--> !disablefirewall = disable windows firewall (requires admin)
--> !audio = play a audio file on the target computer(.wav only) / Syntax = "!audio" (with attachment)
--> !selfdestruct = delete all traces that this program was on the target PC
--> !windowspass = attempt to phish password by poping up a password dialog
--> !displayoff = turn off the monitor(Admin rights are required)
--> !displayon = turn on the monitors(Admin rights are required)
--> !hide = hide the file by changing the attribute to hidden
--> !unhide = unhide the file the removing the attribute to make it unhidden
--> !ejectcd = eject the cd drive on computer
--> !retractcd = retract the cd drive on the computer
--> !critproc = make program a critical process. meaning if its closed the computer will bluescreen(Admin rights are required)
--> !uncritproc = if the process is a critical process it will no longer be a critical process meaning it can be closed without bluescreening(Admin rights are required)
--> !website = open a website on the infected computer / syntax = "!website google.com" or "!website www.google.com"
--> !distaskmgr = disable task manager(Admin rights are required)
--> !enbtaskmgr = enable task manager(if disabled)(Admin rights are required)
--> !getwifipass = get all the wifi passwords on the current device(Admin rights are required)
--> !startup = add file to startup(when computer go on this file starts)(Admin rights are required)
```
## **Advice:**
If you have problems with the installation of win32api or other modules, try installing it in a python virtual environment.\
Please avoid opening issues about module related errors as it is caused by your python installation and not a problem inherent of DiscordRAT.\
If you encounter "AttributeError: module 'enum' has no attribute 'IntFlag'" while compiling to Pyinstaller please do :
```
pip uninstall enum34
```

## **Contact:**
Feel free to contact me if you have any problems.
I also make custom version of this tool (not anymore), so if you want something added feel free to ask by joining by discord server.
https://discord.gg/cKwkkC2U4c.
