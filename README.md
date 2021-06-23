## Root
```sh
$ sudo su
```

## To Uninstall
```sh
# dnf remove rhythmbox -y && dnf remove libreoffice* -y && dnf remove totem -y && dnf remove cheese -y && dnf remove gnome-maps -y && dnf remove gnome-contacts -y && dnf remove gnome-weather -y && dnf remove gnome-boxes -y && dnf remove gnome-photos -y
```

## Free Repos
```sh 
# dnf install https://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm -y
```
## NonFree Repos
```sh
# dnf install https://download1.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm -y
```

## Update OS and repos
```sh
# dnf clean all && dnf update -y && dnf upgrade -y
```

## Reboot
```sh
# reboot
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

## Graphics & Audio
```sh
# dnf install pulseaudio pulseeffects gthumb kdenlive fritzing simplescreenrecorder vlc audacity inkscape gimp -y
```

## Utils
```sh
# dnf install lyx alien gparted gnome-tweak-tool alacarte transmission telegram -y 
```

## Games
```sh
# dnf install steam lutris -y
```

## Dev

```sh
# dnf install java-latest-openjdk.x86_64 -y
```

```sh
# dnf install nodejs npm PyQt5 qt5-designer.x86_64 -y
```

### PHP
```sh
# dnf install httpd curl git unzip php-cli composer php-mysqli php php-zip php-mysqlnd php-mcrypt php-xml php-mbstring -y
```

### LARAVEL
```sh
# cd /var/www/
# git clone https://github.com/laravel/laravel.git
# cd /var/www/laravel
# composer install
```

### MySQL - Before Install

```sh
# dnf install mecab proj libzip pcre-cpp -y
```
```sh
# dnf install mariadb-server -y
# systemctl start mariadb.service
# mysql_secure_installation
```

## Other

- [Visual Studio Code](https://code.visualstudio.com)
- [OBS Studio](https://obsproject.com/wiki/install-instructions#fedora-installation-unofficial)
- [NoiseTorch](https://github.com/lawl/NoiseTorch/releases)
- [GitKraken](https://www.gitkraken.com/download/linux-rpm)
- [Unified Remote](https://www.unifiedremote.com/download/other#linux)
- [Discord](https://github.com/RPM-Outpost/discord)
- [Chrome](https://www.google.com/chrome/?platform=linux)
- [Eclipse](https://www.eclipse.org/downloads)- 
- [TeamViewer](https://www.teamviewer.com/pt-br/download/linux)
- [Slack](https://slack.com/intl/pt-br/downloads/linux)
- [Stremio](https://www.stremio.com/downloads)
- [QtUnified](https://download.qt.io/official_releases/online_installers)
- [Rats](https://github.com/DEgITx/rats-search)
- [Anaconda](https://www.anaconda.com/products/individual)
- [MySQL Workbench](https://dev.mysql.com/downloads/workbench)
- [Java](https://docs.fedoraproject.org/en-US/quick-docs/installing-java)


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

# Nativefier: create webapps
*Must have nodejs and npm installed*

```sh
$ sudo npm install nativefier -g
```
```sh
$ nativefier --name "Web WhatsApp" "https://web.whatsapp.com"
```
```sh
$ nativefier --name "LibreFlix" "https://libreflix.org"
```
```sh
$ nativefier --name "YouTube" "https://www.youtube.com"
```
```sh
$ nativefier --name "YouTube" "https://www.youtube.com"
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

## Config VS Code

- Omni Theme
- Material Icon Theme

### Use CTRL + P (Preferences: Open Settings)
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
