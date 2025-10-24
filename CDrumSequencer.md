# This page focuses on the CDrumSequencer component of my project

The CDrumSequencer handles sequencing of drum hits based on score files. It reads XML-formatted drum patterns and schedules hits for playback over a specified duration. In this case, a "Victory for MSU!" based XML score file. 

Ownership: This sequencer was developed by Shae Killian

Main functionalities of this class:
- Stores drum hits in a std::vector.
- Supports adding hits dynamically via addHit().
- Generates the final audio sequence to WAV via generateSequence(), optionally applying effects. When working with my reverb effect, I found the cymbal feature of my drum kit to be very overbearing,
  so I included a true/false flag that determined whether cymbal was to be indluded or not. 
- Caches loaded WAV samples to reduce redundant file reads.

Supported Grading Elements:
- Reads score files in XML format with loadHitsFromXML() function
- supports multiple instruments in a sequence (full drum-kit)
- variable timing and velocity for hits
- generates full WAV sequences with generateSequence() function

Here is a snippet of this component in use:
CDrumSequencer sequencer;
sequencer.addHit("kick_drum.wav", 0.0, 1.0);
sequencer.addHit("snare_drum.wav", 0.5, 0.8);
sequencer.generateSequence("track.wav", 15.0, &reverbEffect);
