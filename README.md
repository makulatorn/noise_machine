# Noise_Machine V3
The Noise_Machine is a self contained instrument made in Pure Data
It's designed with noise and power electronics in mind and is essentially a collection of different patches taken from different tutorials.
It's made for a noise/power electronics project of mine, but it sounds really cool and i want to share it ✨

Feel free to use it for whatever and modify it to your own needs! ✨

## adc~
Possible to run any kind of instrument or microphone through a soundcard and into the Noise Machine

## Reverb
Made using the freeverb~ object
### Size
Increases/decreases the size of the reverb
### Wet
Controls the wet signal
### Dry
Controls the dry signal
### Damp
A lowpass filter to tame the high frequencies a bit
### Freeze
Freezes the wet signal, disabling the other functions

## Feedback loop
A simple delay that loops for some sweet sweet feedback
Takes whatever input you give it with the inlet but it also has an osc for extra nastyness
### Time
Increases/decreases the time of the delay
### Freq
Sweeps between 0-127Hz (bound to change)
### Feedback
Controls the feedback of the delay
### Vol
Controls the volume, even though it can't really be contained 

## Sequencer
A simple sequencer that randomly generates a new beat every 2 bar
Inside the Drum_samples subpach you can choose a .wav file for it to load and play 
### On/off
Turns the sequencer on and off
### BPM 
Controls the BPM of the sequencerity as the sequencer, but quick and dirty 
Also it just 4 to the floor

## Kick
A very simple oscillator that produces a kick sound
same functional

## Sound & Databend
Takes the binary values from any file on your PC and treats them as a list of amplitudes in an audio file
Mainly makes aggressive white noise, but is great for creating textures, samples and even rythm!
It can also play good ole' .wav files 
### Databend BPM
Increases/decreases the BPM of the databend and sound object, can affect pitch of the sound
### On/Off
Turns the sound & databend object on/off
### Hit
Plays the audio one (1) time

## Complex FM oscillator
Two sine oscillators
Oscillator 1 modulates oscillator 2
Feedback to FModulate oscillator 1

## Wavefolder
Wavefolder with two gain controls, post and pre gain
Most of the different elements go through the wavefolder
Has a display to visualize how the waveform folds

## Input trigger
Takes the input from your soundcard or built-in mic from a laptop and adds a delay and an oscillator, after a certain threshold, for some nice textures
Uses samphold~ to sample its left input whenever the right input decreases in value 
