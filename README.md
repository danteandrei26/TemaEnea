# TemaEnea

The main function of this app is to record the desktop as it starts to perform some tasks:
- Start the web browser (in this case: Google Chrome), accept cookies and goes to www.youtube.com
- Clicks random video (not that random, after version 1.3, the randomness has been removed), waits for the add to pass then starts the audio recording function.
- After a certain amount of time (30 seconds of audio recording in version 1.3), the whole browser stops and the sound file is shown on a graph in dBFS over samples.

Before starting the code, make sure you have installed all modules correctly (+ the webdriver for selenium and Microsoft Visual C++ v14.0 Build Tools for PyAudio).
In order for the app to record the output signal (not microphone which is considered input signal), go to Control Panel >> Hardware and Sound >> Sound > Change system sounds >> Recording: There Enable Stereo Mix and set it as default (The Microphone should switch to <Ready>).
Now you can start the script.

NOTE! The app should run once before plotting the audio file, for some reason it does not detect the file generated on the first try. The file needs to be there first, even if its empty (<output_sound.wav>)
