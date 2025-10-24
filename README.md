# Title: DrumSynthProject-shaekillian

This is the "website" deliverable of the synthesizer project 1 for my DrumSynth project.
I completed this project solo, therefore the only group members included were myself, Shae Killian. 

The format of my score file was XML, which I have included below. When creating the more skeleton-like version of my project, I used a more simple XML score file that was simply testing my projects ability to output any sounds, so I started off a bit more simple. As I was working to fine tune my project, I decided I wanted to challenge myself a bit more by seeing if I could output a familiar song. To do this, I tried asking Generative AI, ChatGPT specifically, to try and create an XML file that followed the drum kit beats of MSU's fight song "Victory for MSU!". However, in my opinion the output does not sound necessarily similar to the song, I still really liked it and decided to keep it as my final project output. I would compare my musical output to an "EDM" type of music, very beat-heavy. 

Here is my drum_pattern.xml:
<pattern>
	<!-- Kick on strong beats -->
	<hit sound="kick_drum.wav" time="0.0" velocity="1.0"/>
	<hit sound="kick_drum.wav" time="1.0" velocity="0.9"/>
	<hit sound="kick_drum.wav" time="2.0" velocity="1.0"/>
	<hit sound="kick_drum.wav" time="3.0" velocity="0.9"/>

	<!-- Snare on backbeat -->
	<hit sound="snare_drum.wav" time="0.5" velocity="0.8"/>
	<hit sound="snare_drum.wav" time="1.5" velocity="0.8"/>
	<hit sound="snare_drum.wav" time="2.5" velocity="0.9"/>
	<hit sound="snare_drum.wav" time="3.5" velocity="0.9"/>

	<!-- Toms for fills -->
	<hit sound="tom_low.wav" time="0.75" velocity="0.6"/>
	<hit sound="tom_high.wav" time="1.25" velocity="0.6"/>
	<hit sound="tom_low.wav" time="2.75" velocity="0.7"/>
	<hit sound="tom_high.wav" time="3.25" velocity="0.7"/>

	<!-- Cymbal accents lightly -->
	<hit sound="cymbal.wav" time="0.0" velocity="0.3"/>
	<hit sound="cymbal.wav" time="2.0" velocity="0.3"/>
	<hit sound="cymbal.wav" time="3.5" velocity="0.4"/>
</pattern>

Generative AI Citations:
Throughout this class, especially when completing the step assignments, I have found it extremely helpful to use AI as tool and reference in helping me complete things I have little experience with. With the steps, I like to prompt it to help create an outline/psuedo for me that gives me the necessary steps I need to include or implement, which helps me stay on track and make sure I am adding every thing needed. I took a similar approach with this project as well. To add another added challenge for myself, I wanted to try and make this project from scratch, rather than using a previous step assignment as my skeleton. To help me with this I asked CHatGPT to create that same outline/guide to help give me a checklist of all specifications and rules I needed to follow, along with what I need to inlcude in my code in order to produce a working project. This was very helpful in creating the skeleton version of my code, which was a simpler version that I used to test different sounds and fine tuning. 

A second challenge I added for myself with this project was, I still wanted to attempt to create a basic effect component, aside from only using it to use my previous wav file as input. I attempted to do this my created a reverb effect. I tried doing this to the best of my ability, and in the output including the reverb effect I can identify the "echo" like reverb sounds, however I do think with more time and effects experience, the reverb could be improved. However, I thought it was extremely fun and challenging to try and take on an added part of this project! Again, for the reverb effect I used AI to assist me in creating another outline stating each aspect I needed to include, as well as for help debugging the issues I was first experiencing with this effect, as it took a lot of "fine-tuning". As you will see, rather than making my reverb effect a menu option like we have previously done in class, I decided to keep them separate and write it only as a function that would be passed in my main.cpp file, to focus on a separation of logic solution, and to help make my final output/solution modular and more clean. Keeping them separate also helped me focus on building the "skeleton" of my project first, then trying to tune it all. 

As stated previously, I used Generative AI to assist me in writing an XML file similar to the song "Victory for MSU!" as well. 
