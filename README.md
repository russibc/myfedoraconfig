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
# dnf install kernel-devel kernel-headers gcc make dkms acpid libglvnd-glx libglvnd-opengl libglvnd-devel pkgconfig -y
```

## Update OS and repos
```sh
# dnf clean all && dnf autoremove && dnf update -y && dnf upgrade -y & reboot
```

## Graphics & Audio
```sh
# dnf install kolourpaint -y && dnf install smplayer -y && dnf install audacity -y && dnf install inkscape -y && dnf install gimp -y
```

## Utils
```sh
# dnf install gparted -y && dnf install gnome-tweak-tool -y && dnf install alacarte -y && dnf install transmission -y && dnf install telegram -y 
```

## Games
```sh
# dnf install steam -y && dnf install lutris -y
```

## Dev
```sh
# dnf install nodejs npm -y
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
- [Chrome](https://www.google.com/chrome/?platform=linux)

## Visual Studio Code Config

- Omni
- Material Icon Theme

```json
{
  "editor.fontFamily": "JetBrains Mono",
  "editor.fontLigatures": true,
  
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
