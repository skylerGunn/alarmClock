# Skyler Gunn 
*requirements: needs to have access to the internal (system clock) or some clock mechanic in order to correctly keep track of time*
*needs to be able to correctly display what time it is in a way that's readable from system data*
*user needs to be able to switch between 2 display modes, 12 hour and 24 hour display*
*user must also be able to adjust the current time via input, and have the clock display the change as well as updating the system clock/time mechanism*
*Additionally, must be able to set 1 or 2 alarms. When the system clock is in sync with that alarm time, will sound alarm until alarm is turned off. If the user hits "snooze", stop alarm and set another alarm for a certain time distance ahead in the future*

![alt text](https://github.com/skylerGunn/alarmClock/blob/master/alarm.png "alarm")

Startup: the alarm is booted up, time is set correctly, and user must set the alarm


| Scenario        | set up alarm and have it go off           |
| ------------- |:-------------:|
| Triggering event      | user hits button that allows them to set alarm |
| Actors      | user input, system clock, system display      |
| Related use cases | display time, update/change clock      |
| Stakeholders           | user, system clock, system display      |
| precondition  | No more than 1 alarm already set |
| postcondition | An alarm is set/ready to go off |

| flow of events | user changes mode to set alarm, system then changes modes and system display displays a change. User then sets their desired alarm time using input buttons and the system records that time for alarm when finished. Alarm goes off when system clock matches the set alarm |
| exception | If more than 1 alarm already set, cannot set another alarm. If user does a "snooze" input after alarm goes off, sets new alarm a set time after snooze |
