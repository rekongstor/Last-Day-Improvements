## XRAY 16 Engine Modifications
## Open X-Ray Call of Chernobyl Edition
----
## Only for Visual Studio 2013
This repository contains XRAY Engine sources based on version 1.6.02 for specific use with the Call of Chernobyl modification.
The original engine is used in S.T.A.L.K.E.R. Call of Pripyat game released by GSC Game World and any changes to this engine are allowed for ***non-commercial*** use only (see [License.txt](https://github.com/avoitishin/xray-16/blob/master/License.txt) for details).

----

- Call of Chernobyl 1.4.22
- Call of Misery 1.0d
- Last Day 1.1 (+ patch from 11.11.17)
- Project name: Last Day Plus Plus (LD++)

----

Current issues you can find in issues.txt

----

Build Instructions:
1) Download xray-16-libraries:
from Yandex.Disk - https://yadi.sk/d/fSU0xaMd3PfpZ5
or Goodle Drive - https://drive.google.com/file/d/1xry3OuVdsHjJpBY8H90BwYRHv3wQwqzW
and unzip them anywhere you want.
2) Open ./src/engile.sln with VS 2013
3) In Property Manager (View\Other windows\Property manager) go to and project (eg xrGame) and in Release | Win32 open Common sheet. Then go to User Macros and change xrLibs directory with your xray-16-libraries\ with \ at the end.
Now you can build with Build Solution. It will compile xrEngine.exe and other .dll's. They will be located in ./bin/bin_rel
- Before copying new files make a backup for original files. 
- Game won't run properly if you won't delete appdata/shaders_cache folder. Also sometimes is required to delete appdata/user.ltx too.

----

There're all the dll's except these ones:
- soft_oal.dll
- wrap_oal.dll
- eax.dll
- lua51.dll

I'm sure soft_oal.dll, wrap_oal.dll and eax.dll are probably modified to make the game do EAX and Open AL Soft stuff on any soundboard.

lua51.dll is located on .\src\3rd party\luajit-2\bin and can be copied to game binaries but that's not thet necessary.

----

Now you can copy fresh compiled files to game/bin directory. Just make sure you made a backup for original bin folder.
Also you need res/gamedata files copied to Last Day gamedata folder.