# RTDSP-Project-2020
Imperial College Year 3 EEE module: Real-time Digital Signal Processing

## Task
We want you to develop a DSP solution that will take an audio input in real time and will detect when different specific sounds are heard. These sounds will be linked to the status of the lift: A- Arriving to a specific floor B- User pressing a button
In your demo you will indicate the detection of the sound by lighting up one of the four LEDs in the DSK board for 1 second.

## Preliminary report
In the preliminary report, we present a list of shortlisted Digital Signal Processing (DSP) methods for detecting in real-time specific sounds in an audio input taken under typical lift conditions, at a sampling frequency of 8kHz. These sounds are less than 1 second long, and belong to two categories - (A) prerecorded speech saying 'First/Second... floor' or (B) a beep from the user pressing a button. We then justify our choice of methods by considering their accuracy, robustness to background noise, speed and calculation burden.

## Final Report
We implemented beep detection using an adaptive frequency amplitude threshold and 'eleven' detection using correlation between frequency spectra. Informal testing showed that our algorithms work satisfactorily in non-noisy situations, but 'eleven' detection is unlikely to be robust to noise. For further improvement, we could combine a noise elimination method with 'eleven' detection or implement a spectrogram-based method for more accurate 'eleven' detection in noisy conditions that has been proven to work effectively on Matlab.
