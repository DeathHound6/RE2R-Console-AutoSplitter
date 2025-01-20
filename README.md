# Resident Evil 2 Remake Console Autosplitter

## Setup
### Downloads
- Download and unzip [LiveSplit](https://github.com/LiveSplit/LiveSplit/releases) (if not already)
    - This AutoSplitter has been tested on version v1.8.29
- Download and unzip [AutoSplit](https://github.com/Toufool/AutoSplit/releases) (if not already)
    - This Autosplitter has been tested on version v2.2.2
    - It is recommend to place this in your LiveSplit folder
- Download the LiveSplit Split file (`.lss`) for your chosen run
    - These are located inside the `Splits` folder
    - Alternatively, you can create the splits yourself, however you must ensure that the ones you make are correct with the given images
    - It is recommended to place this in your LiveSplit folder
- Download the AutoSplit Images folder for your chosen run
    - These are located inside the `SplitImages` folder
    - It is recommended to place this in your LiveSplit folder
- Download the [`LiveSplit.AutoSplitIntegration` component](https://github.com/Toufool/LiveSplit.AutoSplitIntegration/blob/main/update/Components/LiveSplit.AutoSplitIntegration.dll) and save to your LiveSplit's `Components` folder (if not already)

### LiveSplit Setup
- Open LiveSplit
- Right Click LiveSplit and hover over `Open Splits`, and click `From File`. Select the chosen run's LiveSplit Split file (`.lss`)
    - Optionally you may also then select `Edit Splits` to select Difficulty and Platform run variables in the Additional Info tab
    - Once run variables have been set, click `Ok`
- Right Click LiveSplit and select `Edit Layout`
- Click the `+` button, hover over `List`, and click `Splits`
- Click the `+` button again, hover over `Control` and click `AutoSplit Integration`
    - Double click on the newly created `AutoSplit Integration` component
    - Next to `AutoSplit Path`, click on browser, then find and select the `AutoSplit.exe` file
        - This should start AutoSplit
    - Continue to click `Ok` until only the LiveSplit splits and timer are shown
- Right click LiveSplit and click `Save Splits`. Right click LiveSplit again and click `Save Layout`
    - It is recommended to save both to your LiveSplit folder

### AutoSplit Setup
- Within AutoSplit, next to `Split Image Folder`, click browser, and select the images folder for your chosen run
- Click `File`, followed by `Settings`
    - Go to the `Hotkeys` tab
    - Next to `Toggle auto reset image`, click `Set Hotkey` followed by the keyboard key to be used for this hotkey
        - It is recommended to use the same hotkeys that LiveSplit is set to
    - Close the settings window
    - Click `File`, followed by `Save Profile as` and choose a folder to save your AutoSplit settings to
        - It is recommended to save to your AutoSplit folder
- Click `Select Window`, followed by clicking on the window where Resident Evil 2 Remake's video feed is
    - This may be the PC game window, or an OBS window
- Click `Reload Start Image`, and now you should be ready to start running!

## Warnings and Notes
- Due to the nature of this AutoSplitter, being based on video input, it is likely that fake splits will occur
    - This has been attempted to best be mitigated by using the max similarity threshold value for the given time that it *should* split at
    - If a fake split does occur, you may simply use the `Undo` hotkey, or click the `Undo` button on AutoSplit, if available
- It is also possible that splits may not occur when they should
    - In this situation, you may simply use the `Skip` hotkey, or click the `Skip` button on AutoSplit, if available

- Should you need to tweak any settings regarding these images, the details can be found on the [`AutoSplit README file`](https://github.com/Toufool/AutoSplit/blob/main/README.md)
