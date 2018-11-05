# Fleet Week Bird Song

## Sound

Every year in San Francisco, Navy pilots in a group named The Blue Angels fly F-18 jets over the city and around the bay. For the disoriented, this event can be very alarming. A show of USA air supiriority, many residents have visceral reactions to the screaming jets, thunderous roars, angular noise and doppler sound effects.

It's spooky. It makes me think of war and murder and the politics of empire.

It's also totally rad. These jets can fly upside down, ascend nearly vertical and recover from a stall flipping backwards. Four of them fly in formation with the wing tip to cockpit distance around 18 inches. It's a marvel of technology.

I wanted a sound that captures the unease and disorientation of my first Blue Angels encounter. It's repetitious but never repeats. It's stark then alarming. It can fly inverted.

Instruments include

* [Norns FM7](https://github.com/monome/dust/blob/master/scripts/lazzarello/fm7.lua) using algorithm 2
* Electric guitar with [MOD Duo pedal](https://www.moddevices.com/)
* [Mobenthy](http://synthmall.com/ifm/index.html) modular synthesizer
* [Norns PLAYFAIR](https://github.com/monome/dust/blob/master/scripts/tehn/playfair.lua) eucledean drum machine
 
## Process

Much of the jet sounds come from the [Sprott module](https://synthmall.com/ifm/ifmSPR.pdf) from the Mobenthy set. It's based on a term in physics called Jerk, an electrical circuit to demonstrate this natural phenomenon was created by J.C. Sprott in a paper named [A New Chaotic Jerk Circuit](http://sprott.physics.wisc.edu/pubs/paper352.htm). I assume Ieaskul F. Mobenthy read this paper  ;)

The unpredictable triggers on the jerk comes from the [DUNST module](https://synthmall.com/ifm/ifmDUN.pdf), which has a wonderful source of stochastic randomness.

The synth is the Norns FM7 synthesizer using the 2nd algorithm from the Yamaha DX7. I was experimenting with the operator envelopes after I implemented them in the dust software repo. The first operator chain is simple and provides the steady bass loop. The second chain is heavily modified using both the frequency and feedback settings for many of the operators. The envelope for the second chain is much slower to attack then the first but jumps out sharply as it rises. I'm using a lot of "bad sounding" frequency ratios for this operator chain. Some of the spectrum noise is caused by modulation feedback on the sixth operator.

The drums are pretty simple. I found a tempo that had enough range to make a steady beat that blended with the overall tempo and get fast enough to make me feel uneasy. The eucledean pattern generator in PLAYFAIR is awesome. I twist knobs and get polyrhythms!

The guitar are a couple of notes I found late one night after I got home from the bar. I was quite intoxicated. I'm happy with this process. The reverb is from the MOD Duo guitar pedal. It's from the [SHIRO collection of LV2 plugins](https://github.com/ninodewit/SHIRO-Plugins) which appear to have been created in MAX with something called Gen~. I'll have to read up on that. The MOD Duo has a very redumentary looper, which I used for the notes to repeat.

This piece originally came out of me learning some basic recording techniques with the Ardour DAW. I got a fancy Focusrite Scarlett 18i|8 audio interface and a subscription to Ardour builds for macOS. The recording is composed of multiple passes of the instrument loops over the course of a few weeks. It's improvised in that the notes and loops match up based on coincidence. I was modulating some params in realtime. I set a personal rule of "no cutting audio contents in post". I used a few compressors and EQ and clipped the begining and end to points I liked. I did a little volume and pan automation. I mixed the whole thing on headphones.

The final FLAC file was from Audacity. I normalized the volume and applied the equalization effect with the "100Hz Rumble" preset curve. I seem to have trouble getting bass recorded that doesn't sound like mushy dirt.

I'm happy with the result. I'm looking to improve my sensibilities when recording different kinds of instruments. Mixing for different playback systems is not a skill I have right now and would like to develop. I'd also like to improve my ability to reproduce improv setups like this one. I have no way to reproduce this combination of instruments and loops other then by ear, which could be interesting though I wouldn't want to commit to a live performance with an audience using this process.
