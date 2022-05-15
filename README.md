# Shell Scripts
collection of shell scripts I use on my arch install
<br>
i suggest putting them in ~/.local/bin but you can put them wherever you want to as long as it's in PATH
<br>
you can also use them as aliases, if you wish

## gpu
uses nvidia-smi and watch to display some good gpu usage stats

### requirements
 * nvidia-smi

### usage

`gpu`

![gpu example](images/gpu.png)

## nuke
sends SIGKILL to all processes with the name you put in as an arg.
<br>
this is called nuke because it nukes them. all of them. even itself

### requirements
 * none

### usage

`nuke <process>`

![path example image](images/nuke.png)

## path
like `pwd` but you can put a filename in as an argument to get the full path to that file

### requirements
 * none

### usage

`path` 

![example image](images/path1.png)

`path <filename>`

![example image](images/path2.png)


## pip-update
updates all out-of-date python packages with pip. might hang for a bit because `pip list -o` takes some time to list outdated packages

### usage
`pip-update`

![pip-update example image](images/pip-update.png)

## shellcode
uses objdump and some formatting magic to output shellcode for a binary file
<br>
[source](https://www.commandlinefu.com/commands/view/6051/get-all-shellcode-on-binary-file-from-objdump)

### requirements
 * none

### usage

`shellcode <filename>`

![shellcode example](images/shellcode.png)

## spoofmac
uses macchanger to spoof mac address

### requirements
 * systemd
 * NetworkManager
 * macchanger

### usage

`spoofmac <interface>`

![spoofmac example](images/spoofmac.png)

## unspoof
uses macchanger to unspoof your mac address, i.e. set it back to the real one

### requirements
 * systemd
 * NetworkManager
 * macchanger

### usage

`spoofmac <interface>`

![unspoof example](images/unspoof.png)

## targzx
uses `tar` to extract contents of `.tar.gz` into current directory 

### requirements
 * none

### usage

`targzx <filename>`

![targzx example](images/targzx.png)

## tarbzx
uses `tar` to extract contents of `.tar.bz2` into current directory 

### requirements
 * none

### usage

`tarbzx <filename>`

![tarbzx example](images/tarbzx.png)

## youtube
play youtube videos in best quality with mpv

### requirements
 * mpv
 * youtube-dl
   * yt-dlp seems to work a LOT better

### usage

`youtube <link>`

![youtube example](images/youtube.png)

(video resized to fit in my terminal window)
