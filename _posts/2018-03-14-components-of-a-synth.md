---
layout: post
title: Components of a Digital Synth
comments: True
---

## Summary:
* We'll be discussing the different parts of a synth like ES2, Serum, Sylenth, etc.:
    * [Oscillators](#oscillators)
    * [LFO (Technically an oscillator)](#LFO)
    * [Envelopes (ADSR)](#envelopes)
    * [Filters](#filters)
    * [Modulators and Pitch Bends](#modulators)
    * [Effects](#effects)
* Common sounds in EDM produced with synths
    * [Chord Stack - Future Bass](#chords)
    * [Growl - Dubstep](#growl)
    * [808 Bass - Trap](#808)
    * [Airy Pad - Trance](#pad)

## Preface

When I got back from Ultra in March 2017, I became interested in the prospect of making my own music, particularly EDM or Hip Hop. 

<figure>
  <img src="{{site.url}}/assets/pics/ultra.png" alt="ultra" width="400" height="auto">
  <figcaption><em>Why did I choose to wear a fedora, seriously</em></figcaption>
</figure>

I came home ready to become the next Porter Robinson or Steve Aoki, downloaded Ableton and sat down, assuming that I'd be able to create **sick bangers** on the spot. In reality, this is what happened:

<figure>
  <img src="{{site.url}}/assets/pics/confused_boi.jpg" alt="wat dog" width="400" height="auto">
</figure>

I was completely overwhelmed. I knew zero music theory, nothing about composition, or mixing, or mastering, or sound design, or the million other things that went into producing. However, being the tech savvy millenial that I am, I went to Google and typed in "how to make EDM". Many forums mentioned that the foudational skill to creating unique and powerful EDM tracks is sound design. 

But what is __sound design__? According to Wikipedia, 
> Sound design is the art and practice of creating sound tracks for a variety of needs. It involves specifying, acquiring or creating auditory elements using audio production techniques and tools.

In our case, we will be using sound design to create the range of sounds you hear in songs. These sounds can be basses, vocal chops, growls, pads, plucks, risers, effects, or leads. In order to make these, we need a cursory knowledge about the parts of a synth so we can create our own sounds! Let's get into it!

_NB: In most cases, producers will use presets built into synths as a starting point, and then use these tools to modify the sounds into something more unique._

## [Oscillators](#oscillators)

An oscillator is the base of all of our synth work. An oscillator takes a wave form, processes it, and then outputs it to audio format. Without oscillators, a synth is basically a list of effects. There are many types of wave forms, but the basic ones are:

* Saw wave - Sharp tone, used to make supersaws
* Sine wave - Soft tone, used frequently to make basses
* Square wave - Hollow tone, used to synthesize wind instruments
*  Triangle Wave - Sounds something in between a saw and a sine wave, imo

The oscillators will generally have a level wheel, which changes the volume of the oscillator.

Depending on your synth, your oscillator will also be able to add extra voices. Voices can be thought of as copies of your signal. Voices are used in EDM to create supersaws, a type of saw that has 5+ voices that are detuned. This creates a wider, chorus sounding effect.

<figure>
  <img src="{{site.url}}/assets/pics/osc.png" alt="Lodash downloads" width="300" height="auto">
  <figcaption><em>This sound wave is a total square at parties</em></figcaption>
</figure>

## [LFO](#LFO)

An LFO is the bread and butter of EDM production. LFOs give you the wobble we all know and love. It can also be thought of like a mod wheel that moves on its own.

Here is an example of an LFO automating the level (volume) of a supersaw. It's oscillating at 1/8th, meaning it goes through the complete frame in 1/8th note. Pic below.

<audio controls="controls">
  <source src="{{site.url}}/assets/sounds/lfo_example.mp3"></source>
  <p>Your browser does not support the audio element.</p>
</audio>

<figure>
  <img src="{{site.url}}/assets/pics/lfo.png" alt="LFO" width="300" height="auto">
  <figcaption><em>Wub Wub</em></figcaption>
</figure>

## [Envelopes](#envelopes)

Envelopes in synths control ADSR. The easiest way I've seen it explained is on the Image-Line site (the people who make FL Studio). In their [words](http://www.image-line.com/support/FLHelp/html/glossary_envelope.htm):
  
    Attack - The time it takes for the note to reach the maximum level.
    
    Decay - The time it takes for the note to go from the maximum level to the sustain level (the next level in the ADSR chain).
    
    Sustain - The level while the note is held.
    
    Release - The time it takes for the note to fall from the sustain level to zero (silence) when released.

I honestly haven't used envelopes too much in my own productions, but they've definitely come in handy when a sound is clicky (some sounds will have a literal click noise at the start if the attack is too fast). I also use it to mess with release times for pads.

<figure>
  <img src="{{site.url}}/assets/pics/env.png" alt="Envelope" width="300" height="auto">
  <figcaption><em>ADSR = R. SAD???</em></figcaption>
</figure>

## [Filters](#filters)

Filters are used _constantly_. Filters are used to automate risers and create sidechains (that pumping sound you hear in house music). Filters do an amazing job at adding tension, so if you want your track to build suspense, use a _low pass_ filter and raise the cutoff. What this will do is remove the lower frequencies of a sound signal. It's not super important to know the science behind it, but it's worth learning after you get into EQ's as well.

<figure>
  <img src="{{site.url}}/assets/pics/filter.png" alt="Filter" width="250" height="auto">
  <figcaption><em>The most important element in EDM.</em></figcaption>
</figure>

## [Modulators and Pitch Bends](#modulators)

I grouped these two together because they serve similar purposes. They give the artist (you), a manual way to control the structure of a sound. Remember earlier when I said that LFOs were just automated mod wheels? Pitch Bends come super in handy with 808's. 808 basses __love__ to pitch bend. Give it a shot.

<figure>
  <img src="{{site.url}}/assets/pics/mod.png" alt="mod" width="100" height="auto">
</figure>

<figure>
  <img src="{{site.url}}/assets/pics/pitch.png" alt="pitch" width="100" height="auto">
</figure>

## [Effects](#effects)

Effects are fun things that you can add to your sounds you create. When I first got started, I didn't play around with effects too much. This was a huge mistake. I'd say 80% of the character of a sound comes from the effects you apply to it. A boring, flat sound becomes entirely new when you add reverb, delay, or distortion. Some sythns have these built in, on others you'll need to use external plugins or the ones provided with your digital audio workstation.

<figure>
  <img src="{{site.url}}/assets/pics/fx.png" alt="fxEnvelope" width="400" height="auto">
  <figcaption><em>Make those sounds SPICY</em></figcaption>
</figure>

Now onto the fun stuff! Let's make some commonly heard EDM sounds!

## [Chord Stack - Future Bass](#chords)

The chord stack in future bass is the thing you'll hear in pretty much any drop, it does a phenomenal job of creating huge emotions. Luckily, its also pretty easy to make!

Steps:
1. Create a supersaw. We can do this by going to our _oscillator_, increasing the number of _voices_, and _detuning_ the group. Play around with the detuning to find something you like. 
2. Create a LFO, and automate the levels from 0 to 100. This creates that bouncy feel.
3. Create a low pass filter. The only real important part here is to make sure the drive isn't all the way down.
4. Using the same LFO, modulate the cutoff of the filter.
5. Add reverb to taste

Here's how mine looked in Serum. I also added a mod wheel so I could automate the MIDI while it played. The wheel is set to the rate of the LFO, allowing it to move faster or slower when I want it to.

<figure>
  <img src="{{site.url}}/assets/pics/fb.png" alt="Envelope" width="400" height="auto">
  <figcaption><em>Am I Porter Robinson yet?</em></figcaption>
</figure>

And here's what it sounds like:

<audio controls="controls">
  <source src="{{site.url}}/assets/sounds/chord_stack.mp3"></source>
  <p>Your browser does not support the audio element.</p>
</audio>

## [Growl - Dubstep](#growl)

With a growl, our main goal is to create a sound that sounds... grimy. A good growl might remind some people of vomit, but paired with some deep basses it can get people moving on the dance floor. To make a growl:

1. Choose a wavetable that moves around a lot. Ideally, it should change it's character as you move it through the wavetable
2. Create a highpass filter. This is the opposite of the low pass one we discussed earlier, but it serves a similar purpose. It allows the higher frequencies of the growl to pass through, giving the growl that 'voice' that it has. 
3. Creat an LFO and modulate the wavetable position. This is how we take advantage of the crazy wavetables.
4. Add a ton of effects. Seriously. Phasers, distortions, delay, go wild. The sky's the limit here.

<figure>
  <img src="{{site.url}}/assets/pics/growl.png" alt="growl" width="400" height="auto">
  <figcaption><em>Roar.</em></figcaption>
</figure>

<figure>
  <img src="{{site.url}}/assets/pics/growl_fx.png" alt="growl fx" width="400" height="auto">
  <figcaption><em>Roar++.</em></figcaption>
</figure>


And here's what it sounds like:

<audio controls="controls">
  <source src="{{site.url}}/assets/sounds/dubstep_growl.mp3"></source>
  <p>Your browser does not support the audio element.</p>
</audio>

## [808 Bass - Trap](#808)

God, I love a good 808 bass. They're extremely versitale, and often carry entire tracks. They can be distorted, pitch bent(?), legato or short with a heavy attack, you can't really go wrong. The 808 I mainly use is a patch I saw on [Reid Stefan's channel](https://www.youtube.com/watch?v=Yl1SOj_UP-g) on YouTube. Go check him out, he makes great stuff. The important parts of an 808 are:

1. Sine wave oscillator. The 808 is a super smooth bass, and we want a super smooth waveform to match.
2. An LFO with a steep drop off. 808 basses sound a lot like a timpani, which has a super powerful attack and a _long_ release time. 
3. A low pass filter with a modulated cutoff.
4. Pitch Bend! At least 12 semitones.

<figure>
  <img src="{{site.url}}/assets/pics/808.png" alt="808" width="400" height="auto">
  <figcaption><em>I GET THOSE GOOSEBUMPS EVERYTIME</em></figcaption>
</figure>
And here's what it sounds like:

<audio controls="controls">
  <source src="{{site.url}}/assets/sounds/808.mp3"></source>
  <p>Your browser does not support the audio element.</p>
</audio>

## [Airy Pad - Trance](#pad)

Finally, we come to our airy pad. Airy pads add atmosphere to tracks. These are the long, drony, sweet sounding long notes you hear at festivals before the buildups. Pads generally have a long attack time, and they tend to evolve as the notes go along. To make a basic pad:

1. Create a supersaw that is slightly detuned.
2. Adjust the envelope so that the attack and release times go really long.
3. ????
4. Profit.

Here's what I came up with, but as with most things in music, the only rule is that there is no rules.

<figure>
  <img src="{{site.url}}/assets/pics/pad.png" alt="pad" width="400" height="auto">
  <figcaption><em>#sleepysounds</em></figcaption>
</figure>

<figure>
  <img src="{{site.url}}/assets/pics/pad_fx.png" alt="pad_fx" width="400" height="auto">
</figure>

And here's what it sounds like:

<audio controls="controls">
  <source src="{{site.url}}/assets/sounds/pad.mp3"></source>
  <p>Your browser does not support the audio element.</p>
</audio>

## Conclusion

Hope you enjoyed this piece and learned something about digital synths! I've really come to appreciate the effort it takes to create such different sounds in electronic music, and hopefully you'll be inspired to create a sound the world has never heard before.

