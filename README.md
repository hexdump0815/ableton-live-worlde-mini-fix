the worlde mini midi controller is either a clone of the arturia minilab midi controller or is simply the same controller sold under another name/label. out of the box the MiniLab controller definition in ableton 10.1 does not work properly for it. this is a fix for this controller definition to make it work properly. maybe it is also required for the arturia minilab controller itself (i have no such controller, so i cannot test it). 

the files in this repo are based on MiniLab/MiniLab.py of https://github.com/gluon/AbletonLive10.1_MIDIRemoteScripts.git and change the encoder mode from relative_smooth_two_compliment to relative_smooth_binary_offset plus remove the encoder initialization, which seems to put some of the knobs of the controller into a strange mode. the MiniLab.py file should be copied to "Contents/App-Resources/MIDI\ Remote\ Scripts/MiniLab/MiniLab.py" inside of the ableton live app on a mac (right click on the live app in the finder and choose "show package contents") - on windows the remote scripts are located at "\ProgramData\Ableton\Live x.x\Resources\MIDI Remote Scripts\". the modified script will be used then after the next start of live.

thanks a lot to i. for helping to debug the problem.
