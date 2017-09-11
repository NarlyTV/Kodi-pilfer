# Pilfer

Python command line tool to record videos from within Kodi or on the command line

Script requirements:

* git
* python 3.5 
* python 3.5 pip
* ffmpeg 3.0 and above
* rtmpdump 2.4

You also need to install the playercorefacory.xml for your operating system,  
into the kodi userdata directory

* kodi playercorefactory.xml download links 

Location of kodi userdata directory

* Linux ~/.kodi/userdata/
* Mac /Users/<your_user_name>/Library/Application Support/Kodi/userdata/
* Windows Start - type %APPDATA%\kodi\userdata - press return

## Recording from within Kodi

Press y on the keyboard while a video is playing in Kodi to bring up the contextual menu,  
from the menu you can then choose several recording options.

## Script usage on the command line

* video url surrounded by single quotes

```
pilfer -i 'http://example.com/video.m3u8'
```

* text file containing url

```
pilfer -i 'video-url.txt'
```

* recording with duration, 00:00:00 = hours:minutes:seconds

```
pilfer -i 'http://example.com/video.m3u8' -t 00:30:00
```

* text file containing url, recording with duration, 00:00:00 = hours:minutes:seconds

```
pilfer -i 'video-url.txt' -t 00:30:00
```

## Linux set up

### Ubuntu

* Install python 3.6, python3.6 pip, git, ffmpeg, rtmpdump

```
sudo apt install -y python3 python3-pip git ffmpeg rtmpdump
```

### Debian

* Install python 3.6, python3.6 pip, git, ffmpeg, rtmpdump

```
sudo apt install -y python3 python3-pip git-core ffmpeg rtmpdump
```

### Arch Linux

* Install python 3.6, python3.6 pip, git, ffmpeg, rtmpdump

```
sudo pacman -S python python-pip git ffmpeg rtmpdump
```

#### install scripts with pip

```
pip3.5 install --user git+https://github.com/NapoleonWils0n/pilfer.git
```

* upgrade scripts with pip

```
pip3.5 install --upgrade --user git+https://github.com/NapoleonWils0n/pilfer.git
```

## Windows set up

* See t3rmin8tor repo

## Mac set up

### ffmpeg install

[ffmpeg download](https://evermeet.cx/ffmpeg/)

* install ffmpeg

create a folder called bin in your home folder, /Users/your-username/bin

```
mkdir -p ~/bin
```

copy ffmpeg into the ~/bin directory

if you have ffmpeg installed to another location create a symbolic link to $HOME/bin/ffmpeg the same applies to ffplay and ffprobe

then edit your ~/.bash_profile, for example with nano

```
nano ~/.bash_profile
```

and add the code below to your ~/.bash_profile,
which will add any binaries in ~/bin to your bash path

```
if [ -d "$HOME/bin" ] ; then
        PATH="$HOME/bin:$PATH"
fi
```

Then source your ~/.bash_profile

```
. ~/.bash_profile
```

### rtmpdump install

install rtmpdump with homebrew

### install xcode command line tools

* open a terminal and type

```
xcode-select --install
```

### homebrew install

* open a terminal and paste in the code below

```
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

* check brew install

```
brew doctor
```

* rtmpdump install with homebrew

```
brew install rtmpdump
```

### git install

* git download

[git download](https://git-scm.com/download/mac)

### python install

* python download link

[python](https://www.python.org/downloads/mac-osx/)

[python 3.6 download](https://www.python.org/downloads/release/python-362/)

#### install scripts with pip

```
pip3.5 install git+https://github.com/NapoleonWils0n/pilfer.git
```

* upgrade scripts with pip

```
pip3.5 install --upgrade git+https://github.com/NapoleonWils0n/pilfer.git
```

## Freebsd set up

* Install python 3.6, python3.6 pip, git, ffmpeg, rtmpdump

```
sudo pkg install python36 py36-pip git ffmpeg rtmpdump
```

You can also use ports to install the required software

#### install scripts with pip

```
pip3.5 install --user git+https://github.com/NapoleonWils0n/pilfer.git
```

* upgrade scripts with pip

```
pip3.5 install --upgrade --user git+https://github.com/NapoleonWils0n/pilfer.git
```

