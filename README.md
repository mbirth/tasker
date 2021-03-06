Tasker for Android Tasks
========================

(Import by long-press on PROFILES-tab in Tasker.)


CameraMute
----------
Mutes the phone (and therefore the shutter sound) while the camera is active - to not frighten away the subjects.


LetsGoHome
----------
Queries the next transit connection between the given addresses (`%TransitFrom`and `%TransitTo`) and notifies you of the time you should leave. You can set e.g. `%TransitFrom` to `%LOCN` to get directions from your current position.


PowerDownTimer
--------------
Needs a Tasker-compatible motion detection app, e.g. [Motion Detector](https://play.google.com/store/apps/details?id=org.motion.detector Motion Detector). Also needs Root.

Set your desired screen timeout in the `%PowerDownSeconds` variable.

Upon triggering the *Countdown Reset* task, the screen turns on and a green bar appears at the top of the screen and shrinks according to the seconds left. When new movement is detected, i.e. the task is triggered another time, the bar fills up again. If no movement is detected and the bar reaches 0, the screen is turned off.


RainWarning
-----------
Runs upon stopping my morning alarm. It fetches today's weather prediction from Weather Underground
and notifies **ONLY** if there will be rain today.

Don't forget to change `%WUnderKey` to your API key - get one from [here](http://www.wunderground.com/weather/api).

VoiceWeatherAlarm
-----------------
Runs upon stopping my morning alarm. It fetches today's weather prediction from Weather Underground
and speaks it to you aloud. Prediction includes current temperature, sky condition, humidity percentage, day temperature high, and day temperature low. Additional data can be added be reading the wunderground.com api documentation and editing the tasker details.

Don't forget to change `%WUnderKey` to *your* unique API key - get one from [here](http://www.wunderground.com/weather/api). Also, enter in your name and zip code. Detailed instructions can be found 
[here](https://github.com/NA-Dev/VoiceWeatherAlarm-Tasker).

You may need to download a Tasker-compatible alarm app, e.g. [Gentle Alarm](https://play.google.com/store/apps/details?id=com.mobitobi.android.gentlealarm&hl=en). Alternatively, you could give the free [ClockTask](https://play.google.com/store/apps/details?id=com.balda.clocktask&hl=en) plugin a try along with your stock alarm app.


SayCaller
---------
Announces the caller's first name.


SayLocation
-----------
This task aquires your location, geocodes it into an address using the Google Geocoding API and speaks the address to you. It is meant to be launched via Google Now and AutoVoice.
