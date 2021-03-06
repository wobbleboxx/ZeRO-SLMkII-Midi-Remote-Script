# ZeRO-SLMkII-Midi-Remote-Script
MIDI Remote Script for the novation ZeRO SLMkII and Ableton Live

The novation ZeRO SLMkII isn't supported anymore by novation. Also the Automap software is out of date and didn't bring much for customization.
I always wanted to customize the controller to my needs and so this MIDI Remote Script for Ableton Live is what I built.

![Image of the controller showing the different sections used in the script](https://github.com/wobbleboxx/ZeRO-SLMkII-Midi-Remote-Script/blob/master/ControlSheet.png)

### Features overview:

| Controls | Operation |
| --- | --- |
| Ring Encoders | Track Send 1 |
| Poties | Track Pan |
| Pads | Custom Actions (view Custom Actions section) |
| Left side button row 1 | Track solo |
| Left side button row 2 | Clip stop |
| Sliders | Track Volume  |
| Right side button row 1 | Track mute |
| Right side button row 2 | Track arm |

- Transport controls can be enabled with the "transport" button
- Move to next or previous 8 tracks with "preview" + "page" buttons
- The display only shows the track names, no parameter values (use your computer screen for detailed parameter values)
- A track can be selected by pressing it's arm button twice (arm on -> arm off)

### Custom Actions:

| Pad | Action |
| --- | --- | 
| Pad 1 | Toggle metronome on/off |
| Pad 2 | Tap tempo |
| Pad 3 | Save the Live set |
| Pad 4 | Add audio track |
| Pad 5 | Add return track |
| Pad 6 | undefined |
| Pad 7 | Undo |
| Pad 8 | Add MIDI track |

### Support:
- This has only been tested with the novation ZeRO SLMkII
- This has only been tested with Live 9.7.5

### Known bugs:
- Add audio track button is adding a MIDI track
    At this point I have no idea why the function "create_audio_track" is adding a MIDI track.
- Screen is empty or showing "Ableton is OFFLINE" when using the right side controls
    This is to no reason to me as well. I tried for some hours figuring out why this happens, but I think there might be something I don't see in the controller itself.
- Saving the Live set only works on macOS.
    In fact this is not a Live command but the pad is mapped to the shortcut CTRL + S. So if you mapped this shortcut to something else, that is what will be called instead.
- If the controller is turned on after Live is running, sometimes the Remote Script will not run.
    Just turn on the controller before starting Live and it should be fine.

### How to use / install:

1. Download a copy of the "ZeRO_SLMkII" folder
2. Copy the folder into /Applications/Ableton Live 9 Suite.app/Contents/App-Resources/MIDI Remote Scripts/
3. Select the Ableton template on the controller
4. Select "ZeRO_SLMkII" in Live -> Preferences -> MIDI -> Control Surface with the controller input and output on port 1
5. Select "track" and "remote" for the input and output of the MIDI ports

![Image showing the settings in Live](https://github.com/wobbleboxx/ZeRO-SLMkII-Midi-Remote-Script/blob/master/LiveSettings.png)

## Todo:
- Fix the display bug
- Add comments to code

### Note
Feel free to use it on your own, but here are some considerations:
- Use at your own risk
- Modify at your heart's desire; let me know if you built something cool with it :) (not mandatory)