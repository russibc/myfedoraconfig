## Root
```sh
$ sudo su
```

## Remove
```sh
# dnf remove rhythmbox -y && dnf remove gnome-calendar -y && dnf remove cheese -y && dnf remove gnome-maps -y && dnf remove gnome-contacts -y && dnf remove gnome-weather -y && dnf remove gnome-videos -y dnf remove gnome-boxes -y

```

## Update OS and repos
```sh
# dnf clean all && dnf autoremove && dnf update -y && dnf upgrade -y
```

## Graphics & Audio
```sh
# dnf install vlc -y && dnf install audacity -y && dnf install inkscape -y && dnf install gimp -y
```

## Utils
```sh
# dnf install gnome-tweak-tool -y && dnf install alacarte -y && dnf install transmission -y && dnf install chromium -y && dnf install telegram -y 
```

## Games
```sh
# dnf install steam -y
```

## Android Studio 

### Before install
```sh
$ sudo dnf install zlib.i686 ncurses-libs.i686 bzip2-libs.i686 -y
```

- [Android Studio](https://developer.android.com/studio/install#linux)


### Add To Path
```sh
$ export ANDROID_HOME=/home/$USER/Android/Sdk/
```
```sh
$ export PATH=$PATH:$ANDROID_HOME/tools
```

## Other

- [Java](https://docs.fedoraproject.org/en-US/quick-docs/installing-java)
- [GitKraken](https://www.gitkraken.com/download/linux-rpm)
- [Visual Studio Code](https://code.visualstudio.com)
- [Spotify](https://docs.fedoraproject.org/en-US/quick-docs/installing-spotify)
- [Unified Remote](https://www.unifiedremote.com/download/other#linux)
- [Eclipse](https://www.eclipse.org/downloads)
