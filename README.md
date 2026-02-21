# easyCLI 1.0.1 🐍
# ![python](https://img.shields.io/badge/Python-3-blue)

----
CLI python based made by Mainzzz 📜
----
#### Created by: Mainzzz ([my portfolio](mainzkuyyy.vercel.app))
#### Version: 1.0.0
#### Description: Aarch64 Linux Simulator for Mobile

## Directory (.zip) [UPDATED] 📂
```
easyCLI
| main.py
| os
| | installed_package
| | | installed.json
| | sandbox
| package
| command
| | __init__.py
| | filesystem
| | | __init__.py
| | | system.py
| | package
| | | __init__.py
| | | system.py
| | general.py
| | package_loader.py
```
__Context__:
- main.py : os displayer
- os : all system take place (sandbox, installed_package) [MODIFICATION]
- command : command folder
- package : package manager folder [NEW]
- init.py : basic Python module folder identity
- filesystem, system : filesystem command works
- package, system: packaging command works [NEW]
- general.py : all command met
- init.py in command : creates command_map dict to pass on main.py
- package_loader.py : all package command loaded to command_map [NEW]

## Commands 📊
| Command | Description         |
|---------|---------------------|
|`mkdir`  |Creates folder       |
|`touch`  |Creates file         |
|`mv`     |Moving file          |
|`cd`     |Move to specific directory|
|`rm`     |Removes file/folder  |
|`ls`     |Checks all the directory|
|`cp`     |Checks current directory|
|`pkg`    |Package manager [NEW]|

## How to Install 🔽
__In Termux:__
```
pkg install git (if dont have)
pkg install python (if dont have)
git clone https://github.com/mainzkuyyy/easyCLI-v1.0.1
cd easyCLI-v1.0.1
unzip easyCLI.zip
```
__In Pydroid:__
```
1. open Pydroid
2. open Terminal mode in left operrand menu
3. cd ~/storage/emulated/0/Downloads/easyCLI (must be downloaded and unzip manually in file manager)
4. python main.py
```

## Note 📝
Version 1.0.1 is released, `pkg` command works pretty well
Package manager now holds:
```
python
```
You can create yourself package:
1. Create folder in `/package`
2. Name it
3. Create `manifest.json`, and `/app`
4. `manifest.json` structure are in order:
```
{
    "name": "my_package",
    "creator": "myself",
    "version": "1.0.0",
    "description": "This is a my package",
    "app": ["commands.py"] // to hold your costum command
}
```
5. Add `commands.py` inside the `/app`
6. Fill all your system and ends with registering (more at python package i pre-build for you)
7. Test it out, simply:
```
$> pkg install my_package
Installing package...
Install success

$> mycommand test
Hello, this is my command
```
Have fun playing with its thing

### © MainzKuyyy 2026
