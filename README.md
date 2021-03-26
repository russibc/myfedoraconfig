## Root
```sh
$ sudo su
```

## Remove
```sh
# dnf remove rhythmbox -y && dnf remove libreoffice* -y && dnf remove totem -y && dnf remove cheese -y && dnf remove gnome-maps -y && dnf remove gnome-contacts -y && dnf remove gnome-weather -y && dnf remove gnome-boxes -y
```

## Free Repos
```sh 
# dnf install https://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm -y
```
## NonFree Repos
```sh
# dnf install https://download1.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm -y
```
## Essential

```sh
# dnf groupinstall 'Development Tools' -y
```

```sh
# dnf install gnome-font-viewer kernel-devel kernel-headers gcc make dkms acpid libglvnd-glx libglvnd-opengl libglvnd-devel pkgconfig libcurl-devel sqlite-devel libnotify-devel -y
```

```sh
# curl -fsS https://dlang.org/install.sh | bash -s dmd
```

## Update OS and repos
```sh
# dnf clean all && dnf autoremove && dnf update -y && dnf upgrade -y & reboot
```

## Graphics & Audio
```sh
# dnf install kolourpaint smplayer audacity inkscape gimp -y
```

## Utils
```sh
# dnf install alien gparted gnome-tweak-tool alacarte transmission telegram -y 
```

## Games
```sh
# dnf install steam lutris -y
```

## Dev
```sh
# dnf install nodejs npm pyqt5 qt5-devel qt-creator -y
```

## Android Studio 

### Before install
```sh
# sudo dnf install zlib.i686 ncurses-libs.i686 bzip2-libs.i686 -y
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
- [Unified Remote](https://www.unifiedremote.com/download/other#linux)
- [Eclipse](https://www.eclipse.org/downloads)
- [Chrome](https://www.google.com/chrome/?platform=linux)
- [TeamViewer](https://www.teamviewer.com/pt-br/download/linux)
- [Slack](https://slack.com/intl/pt-br/downloads/linux)
- [Stremio](https://www.stremio.com/downloads)
- [OneDrive](https://github.com/skilion/onedrive)
- [Astah](https://astah.net/downloads)

# Spotify

- [Spotify](https://docs.fedoraproject.org/en-US/quick-docs/installing-spotify)

## If it fails, workaround:

```sh
$ mkdir spotify
```
```sh
$ cd spotify
```
```sh
$ wget http://repository-origin.spotify.com/pool/non-free/s/spotify-client/spotify-client_1.1.42.622.gbd112320-37_amd64.deb
```
```sh
$ sudo gedit /usr/share/lpf/packages/spotify-client/spotify-client.spec
```

### Change global variable, save and close Text Editor
%global repo        http://localhost:8000

```sh
$ python -m http.server
```

### In another terminal
```sh
$ sudo dnf update lpf-spotify-client
```

# Visual Studio Code

- [Visual Studio Code](https://code.visualstudio.com)

## Config 

- Omni
- Material Icon Theme

```json
{
  "editor.fontFamily": "JetBrains Mono",
  "editor.fontLigatures": true,
  "terminal.integrated.fontFamily": "Source Code Pro",
  "workbench.colorTheme": "Omni",
  "workbench.iconTheme": "material-icon-theme",
  "workbench.startupEditor": "newUntitledFile",

  "explorer.compactFolders": false,
  "editor.renderLineHighlight": "gutter",
  "workbench.editor.labelFormat": "short",
  "extensions.ignoreRecommendations": true,

  "javascript.updateImportsOnFileMove.enabled": "never",
  "typescript.updateImportsOnFileMove.enabled": "never",

  "breadcrumbs.enabled": true,
  "editor.parameterHints.enabled": false,
  "editor.formatOnSave": true,
  "explorer.confirmDragAndDrop": false,
  "explorer.confirmDelete": false,
  
  "emmet.syntaxProfiles": { "javascript": "jsx" },
  "emmet.includeLanguages": { "javascript": "javascriptreact" },

  "javascript.suggest.autoImports": true,
  "typescript.suggest.autoImports": true
}
```
