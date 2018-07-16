# Grasp-and-Lift-detection-from-EEG

The goal of this study is to develop an EEG movemnt decoder that detects 6 kinds of hand movements from 32 channels EEG data (sampling rate 500Hz).
There are 12 subjects in total, 10 series of trials for each subject, and approximately 30 trials within each series. <br>
The 6 hand events mimic the grasp-and-lift movement in sequential order: 
1. HandStart
2. FirstDigitTouch
3. BothStartLoadPhase
4. LiftOff
5. Replace
6. BothReleased

## Additional consideration
The application of this algorithm is real-time brain-machine interface (BCI), which requires on-line computing. This also adds a time-series constraint where prediction can't be based on future data. <br>

The spatial relationship between the electrode locations is shown in this diagram:
![eeg_electrode_numbering](https://user-images.githubusercontent.com/30357662/42740941-8968cc94-887b-11e8-8ceb-a9cfc33075f7.jpg)
