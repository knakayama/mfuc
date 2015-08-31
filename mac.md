Mac
===

```bash
$ qlmanage -p <image>
```

```bash
$ screencapture -c <image>
$ screencapture -i <image>
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
