# Lab 7 — ThingSpeak and Google Sheets
## Part 1
I ran thingspeak_cpu_loop.py and thingspeak_feed.py in a demo folder to collect and upload data about my cpu performance.
```console
PS C:\Users\marci\downloads\iot\lesson7> py thingspeak_feed.py
An API key savefile was not found. Enter Write API Key >>> P56MOPYM5YMSAOMS
Should we save this key for future use? [y/N] >>> y
8.2
2361.6953125
Sun, 13 Apr 2025 21:32:15
200 OK
8.2
2101.83984375
Sun, 13 Apr 2025 21:33:15
200 OK
7.3
2216.12890625
Sun, 13 Apr 2025 21:34:15
200 OK
6.1
2607.625
Sun, 13 Apr 2025 21:35:15
200 OK
6.2
2694.0234375
Sun, 13 Apr 2025 21:36:15
200 OK
13.1
3043.5703125
Sun, 13 Apr 2025 21:37:15
200 OK
5.0
3599.984375
Sun, 13 Apr 2025 21:38:15
200 OK
```

## Part 2
I installed gspread and oauth2client, and created a new Google Cloud Platform service account with a JSON key file, in order to use Google SHeets API calls. By prepping a new sheet and running cpu_spreadsheet.py, I was able to upload the data collected in Part 1 to Google Drive.
```console
C:\Users\marci\iot\lesson7> py rpi_spreadsheet.py
Free RAM: 16 (866)
Number of processes: 178
Up time:  9:40
Number of connections: 2
Temperature in C: 63.3
IP-address: 192.168.1.181
CPU speed in MHz: arm_freq=1500

Logging sensor measurements to rpidata every 10 seconds.
Press Ctrl-C to quit.
2025-04-13 21:40:49.034073
CPU Usage:   21.2 %
Temperature: 63.7 C
Wrote a row to rpidata
2025-04-13 21:40:59.234427
CPU Usage:   15.2 %
Temperature: 62.8 C
Wrote a row to rpidata
2025-04-13 21:41:09.402127
CPU Usage:   14.1 %
Temperature: 63.3 C
Wrote a row to rpidata
2025-04-13 21:41:19.572112
CPU Usage:   15.3 %
Temperature: 62.3 C
Wrote a row to rpidata
2025-04-13 21:41:29.762102
CPU Usage:   15.3 %
Temperature: 62.8 C
Wrote a row to rpidata
2025-04-13 21:41:39.973860
CPU Usage:   15.1 %
Temperature: 63.7 C
Wrote a row to rpidata
```
