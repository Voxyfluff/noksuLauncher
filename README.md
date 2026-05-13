# noksuLauncher
simple multi-program launcher to make launching multiple apps at once very simple. originally made for [Noksuna](https://twitch.tv/noksuna).

1. download the newest .exe file from the [Releases](https://github.com/voxyfluff/noksuLauncher/releases) and save in a new folder
2. run the .exe file
3. add the wanted programs by pressings the Browse button, or enter a steam rungame link (eg. steam://rungameid/620 for portal 2)
4. check the checkboxes next to the programs that should be launched
5. hit Launch Selected
since update v2 you can add more program slots by opening the config file and editing the "indexes" property. it has been proven that everything between 5 and 20 works, everything else bugs the UI.

note: windows might throw an error about the application not being verified. thats because I do not have $250 to spend every year just for that popup to not pop up. if that warning scares you into not using the program: the source code is public in this repository, go read that and see if you find anything malicious.

# known problems
- when launching steam apps via steam://rungameid/{appid} with arguments it shows up as "Steam App --{arg}" (example: steam://rungameid/438100/--no-vr shows up as Steam App --no-vr instead of VRChat)
- errors out trying to remove a temporary directory after closing the launcher
