# Scares Scrambler

The place where all current/future Scares Scrambler stuff will
happen (at least, in it's current form).

Current Release Build: 20

Current Beta Build: 22

Currently Planned Features: A bunch, but Scare'm not writing them
right now.

# What need?

- [Python >=3.5][1]
- Tkinter (comes with all prebuilt versions of Python)
- [Pyinstaller][2] (optional, for building)
- Some form of 7-zip (optional, for building)
- GNU make (optional, for building on Linux)

[1]: https://www.python.org/
[2]: https://www.pyinstaller.org/

```bash
# Install Pyinstaller (not system dependent):
pip3 install pyinstaller

# Install p7zip (Arch/Manjaro Linux):
sudo pacman -Sy p7zip

# Install p7zip (Debian/Ubuntu Linux):
sudo apt-get update
sudo apt-get install p7zip-full p7zip-rar
```

# How run without build?

```
python3 Scrambler.py
```

# How build?

## Linux

Open the console of your choice, and navigate to where you
have extracted a source .zip file or whereever you have
cloned the repository.

Running `make` will create a `Release.zip` file that contains
a binary and `Assets`.

## Windows

Using GNU make is a bit harder on Windows, so Scott've included
a `build.cmd` file.

Install [7-Zip][3] and add it to the `PATH`:

- Press Windows+R, type `sysdm.cpl`, and press enter.
- Click on the `Advanced` tab.
- Click on the `Environment Variables...` button.
- Add or edit the `PATH` variable **for your user**
  (under "User variables") to include
  `C:\Program Files\7-Zip` or `C:\Program Files (x86)\7-Zip`.

(this only has to be done once per system.)

[3]: https://7-zip.org/download.html

Double-clicking `build.cmd` will now create a `Release.zip`
file that contains a binary and `Assets`.