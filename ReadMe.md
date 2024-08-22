# aurioTouch & avTouch

## [aurioTouch](https://developer.apple.com/library/archive/samplecode/aurioTouch/Introduction/Intro.html)

aurioTouch demonstrates use of the remote i/o audio unit for handling audio input and output. The application can display the input audio in one of the forms, a regular time domain waveform, a frequency domain waveform (computed by performing a fast fourier transform on the incoming signal), and a sonogram view (a view displaying the frequency content of a signal over time, with the color signaling relative power, the y axis being frequency and the x as time). Tap the sonogram button to switch to a sonogram view, tap anywhere on the screen to return to the oscilloscope. Tap the FFT button to perform and display the input data after an FFT transform. Pinch in the oscilloscope view to expand and contract the scale for the x axis.

The code in aurioTouch uses the remote i/o audio unit (AURemoteIO) for input and output of audio, and OpenGL for display of the input waveform. The application also uses AVAudioSession to manage route changes (as described in the Audio Session Programming Guide).

## [avTouch](https://developer.apple.com/library/archive/samplecode/avTouch/Introduction/Intro.html)

The avTouch sample demonstrates use of the AVAudioPlayer class for basic audio playback.

The code in avTouch uses the AV Foundation framework to play a file containing AAC audio data. The application uses Core Graphics and OpenGL to display sound volume meters during playback.

This application shows how to:

* Create an AVAudioPlayer object from an input audio file.

* Use OpenGL and Core Graphics to display metering levels.

* Use Audio Session Services to set an appropriate audio session category for playback.

* Use the AVAudioPlayer interruption delegate methods to pause playback upon receiving an interruption, and to then resume playback if the interruption ends.

* Demonstrates a technique to perform Fast Forward and Rewind

avTouch does not demonstrate how to play multiple files, nor does it demonstrate more advanced use of AV Foundation.