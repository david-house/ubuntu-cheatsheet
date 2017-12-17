# ubuntu-cheatsheet
Reminders for useful ubuntu commands

## List the attached network adapters and some properties in XML
```
sudo lshw -C network -xml
```

## Change the wireless card from managed to monitor mode and log to XML
```
sudo /usr/sbin/airmon-ng start <interface name ex.: wlx00...>
sudo /usr/sbin/airodump-ng -w /home/pi/airodump_logs/log --band abg --manufacturer --output-format netxml --output-format gps --gpsd <renamed interface ex.: wlan1mon>