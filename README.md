calendar-patch
==============

"The calendar was broken, so I fixed it."

#calendar.patch
 - Fixes wrong date being set when adding events between 23 an 00
 - Makes end time be reset to one hour after the start time when adjusting start time
    (Same as before, just adjusts the date too if needed, not only the time)

#ClockAlarmDialog.patch
 - Makes a timed-out alarm trigger the same action as a snooze
 
