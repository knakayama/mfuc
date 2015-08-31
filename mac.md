Mac
===

```bash
$ qlmanage -p <image>
```

```bash
$ screencapture -c <image>
$ screencapture -i <image>
# Capture the contents of the screen, including the cursor, and attach the resulting image to a new Mail message
$ screencapture -C -M <image>.png
# Select a window using your mouse, then capture its contents without the window's drop shadow and copy the image to the clipboard
$ screencapture -c -W
# Capture the screen after a delay of 10 seconds and the open the new image in Preview
$ screencapture -T 10 -P <image>.png
# Select a portion of the screen with your mouse, capture its contents, and save the image as a pdf
$ screencapture -s -t pdf <image>.pdf
```

```bash
$ sips --resampleWidth 100 <image> --out <image>
```

```bash
# http://www.cyberciti.biz/faq/apple-macosx-disable-sleeping-from-bash-command/
# Prevent the display from sleeping
$ caffeinate -d
# Prevent the system from idle sleeping
$ caffeinate -i
# Prevent the disk from idle sleeping
$ caffeinate -m
# Prevent the system from sleeping when system is running on AC power
$ caffeinate -s
# How do I declare that user is active?
$ caffeinate -u vivek
$ caffeinate -u vivek wget url
# How do I set timeout?
$ caffeinate -t 60
$ caffeinate -t 120 wget url
```

```bash
# http://www.cyberciti.biz/faq/howto-restart-airport-wireless-from-bash-command-line-in-macosx/
$ sudo ifconfig en0 stop
$ sudo ifconfig en0 start
$ sudo ifconfig -u en0
# Restart Mac OS X networking
# off
$ networksetup -setairportpower en0 off
$ networksetup -setairportpower 'Wi-Fi' off
# on
$ networksetup -setairportpower en0 on
$ networksetup -setairportpower 'Wi-Fi' on
```

```bash
# http://other-zbx1.sakura.ad.jp/zabbix/screens.php?sid=40a24461748c1a5b&form_refresh=1&fullscreen=0&elementid=97
# -a: to choose the app yourself
$ open -a
# -e: to open the file for editing in TextEdit
$ open -e
# mdfind: locate alternative
$ mdfind
$ diskutil list
```
