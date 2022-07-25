# tailscale-systray

Linux port of tailscale system tray menu.

![tailscale-systray](/screenshot.png)

## Usage

```
$ tailscale-systray
```

## Requirements

* tailscale

## Installation

### Install requirements

Building app require gcc, libgtk-3-dev, libappindicator-3-dev

```
sudo apt-get install gcc libgtk-3-dev libappindicator3-dev
```
Building app which worked for me with following system conditions
  (
  - Operating System: Kubuntu 22.10
  - KDE Plasma Version: 5.25.3
  - KDE Frameworks Version: 5.96.0
  - Qt Version: 5.15.4
  - Kernel Version: 5.16.0-051600-generic (64-bit)
  - Graphics Platform: X11
  ) 

```
sudo apt-get install gcc libgtk-3-dev libayatana-appindicator3-dev

sudo ln -s /usr/lib/x86_64-linux-gnu/pkgconfig/ayatana-appindicator3-0.1.pc /usr/lib/x86_64-linux-gnu/pkgconfig/appindicator3-0.1.pc
```

### Install app

```
go install -v github.com/mattn/tailscale-systray@latest
```

At this point you can start it with `tailscale-systray`.

### Run at startup

You can do this in different ways. One option is to add the command to "Startup Applications" if your system has it:

![tailscale-systray startup](/screenshot_startup.png)

## License

MIT

Icon file is copied from official repository.

## Author

Yasuhiro Matsumoto
