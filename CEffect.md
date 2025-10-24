# This file is focused on the Reverb effect of my project, CEffect

The CEffect class implements a simple delay-based reverb effect. It takes the output of the drum sequencer as input and applies a wet/dry mix. 
The class uses a circular buffer to store delayed samples and mixes them with the original input to create a reverb tail. While the effect was applied successfully, 
cymbal hits were often too loud and caused clipping, so the sequencer was modified to exclude cymbals when generating the reverb version of the track.

Ownership: this effect was developed by Shae Killian

Key Features Implemented:
- 300ms delay buffer to produce a reverb tail
- Wet/dry mix control (setWetDryMix())
- Feedback loop to sustain reverb
- Circular buffer to manage delayed samples

Supported Grading Elements:
- Takes output from synthesizer/sequencer as input
- Processes audio in real time (streaming)

Each component within this project works sample-by-sample and outputs immediately, to ensure the entire audio pipeline is streaming.

Limitations/Notes:
- Cymbals were excluded from the reverb track to avoid clipping and overpowering the rest of the output
- This effect is very basic, as I was just trying to challenge myself in having a working reverb output, no necessarily the most complex or a multi-tap reverb
  
