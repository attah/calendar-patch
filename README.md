calendar-patch
==============
```
  __  __               __                                               _     __     
 / / / /__ ___   ___ _/ /_  __ _____  __ ______  ___ _    _____    ____(_)__ / /__   
/ /_/ (_-</ -_) / _ `/ __/ / // / _ \/ // / __/ / _ \ |/|/ / _ \  / __/ (_-</  '_/   
\____/___/\__/  \_,_/\__/  \_, /\___/\_,_/_/    \___/__,__/_//_/ /_/ /_/___/_/\_\    
                          /___/                                                      
```
"The calendar was broken, so I fixed it."

Apply with patch -p0 -i <patchfile>

#calendar.patch
 - Fixes wrong date being set when adding events between 23 and 00
 - Makes end time be reset to one hour after the start time when adjusting start time
    (Same behavior as before, just adjusts the date too if needed, not only the time)
 - Sets default reminder for new events to 15 minutes

#ClockAlarmDialog.patch
 - Makes a timed-out alarm trigger the same action as a snooze
 
