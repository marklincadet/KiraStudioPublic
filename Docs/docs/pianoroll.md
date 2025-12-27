# Overview

The **Piano Roll** is where you enter notes inside of patterns and likely where you will be spending most of your time in the app.

The piano roll is makde of a few components:

* On the left is the **Vertical Piano** which can be used to preview the instrument of the selected channel. Note that the selected channel may not necessarely be the one being edited.
* On the top is the **Timeline** which display the beats in a `Bar.Beat` format.
* In the middle is the piano roll itself where notes are edited.
* At the bottom is the **Note Parameter Editor** where extra note parameters (velocity, pan, aftertouch, etc.) can be edited.
* In the top-right corner is the **Floating Toolbar** which contains various snapping and view options.

![](images/PianoRoll.png#center)

Unlike other apps like FL Studio, the piano roll does not only show you the notes of the current pattern in a vacuum, it displays a continuous view of a track. Notes can be freely moved from one pattern to another. Notes can extend beyong the end of a pattern, but they belong to the pattern where they start from.

# Editing Notes

We will focus our attention to the center of the piano roll where all the notes lie.

## Adding & deleting notes

To add a new note, simply click on an empty space.

* On desktop, you can click and drag to adjust the final position of the note.
* On mobile, it just a tap.

On all platforms, deleting single notes is achieve by double-clicking. **Shift-Click** is also an alternate option on desktop.

## Selecting notes

Selected notes have a white outline around them and can be modified as a group.

* On desktop, you can select notes by right-clicking in the background and dragging to drag a rectangle. 
* On mobile, you can longpress in the background and start drawing a rectangle once the pulsating circle appears. 

You can also select a time range of notes by doing a selection from the timeline, which is the row with the bar/beat numbers at the top.

## Moving, transposing & resizing notes

To move notes simple click and drag. When starting a drag from a selected note, all the selected notes will together.

* On desktop, notes can be resized by grabbing the left or right side edge and dragging. Desktop can also move notes using the arrow keys. Pressing up/down will transpose by 1 semitone or 1 octave if **Ctrl** is held at the same time. Pressing left/right will move by the amount of the currently selected snapping precision.
* On mobile, notes are resized by using one of the big colored resize handle.

## Duplicating notes

When there are more than 1 note selected, the entire selection can be duplicated by dragging from the **Colored Paperstack Icon** that appears and release it where you want to create the copy. On desktop, the same can also be accomplished by pressing and holding **Ctrl** while dragging notes.

> TODO : A mobile/desktop GIF here would be nice.

## Snapping to beats

Snapping to beats can be toggled from the floating toolbar on the right and the precision can be adjusted. 

The snapping precision is expressed in beats. This mean that in a 4/4 time signature, for example, snapping to 1/4 Beat snaps to 1/16th notes.

## Slide notes

Slide notes are notes that start at a given pitch (the pitch of the note) and slowly change to hit a target pitch which is represented by where the triangle ends.

> TODO : Image here.

To create a slide note, simple select one of the 3 slide note mode from the contextual menu that appears when right-clicking (long-pressing on mobile) on a note. 

There are 3 types of slide notes:

* **Note Linear** : This is roughly the equivalent of doing a glissando on a piano. The note value itself (ex: A4 to A5) will be interpolated, leading to a natural sounding slide. Unless you are trying to achieve a specific retro or chiptune effect, use this mode.
* **Frequency Linear** : This will interpolate the frequency of the note (ex: 440Hz to 880Hz) and use the result as the final frequency. 
* **Period Linear** : This will interpolate the period (ex: 1/440Hz to 1/880Hz) and use this as the final frequency. This mode is particularly useful to mimic the behavior of retro/chiptune slides.

The frequency and period linear modes will display a convex or concave slide note. Please note that this is simply a rough visual cue and does not accurately represent the pitch of the note that will actually play. 

The target and duration of a slide note can be modified by dragging the **Four-Arrows Icon** that will appear if a slide note is present. 

* When using the [note end release mode](#release-modes), slide notes can extend beyond the release of the note, as sound can still be heard during the release. 
* When using the [manual release mode](#release-modes), slide notes we be required to end exactly at the end of the note, as this represent a hard-kill. When using the 

## Disabling attack

By default, notes have an attack which mean they will restart their envelopes from the beginning. 

The attack can be toggled for a particular note by selecting the **Toggle Note Attack** option from the contextual menu that appear when right-clicking (long-pressing on mobile). 

Notes with no attack will show an ellipsis (...) before their value.

> TODO : Image here.

Disabling the attack in the piano roll does not mean it will always work, there are a few rules to understand on how the audio player uses them. 

Generally speaking, when the player encounter a note without attack, it will look for a previous note still producing sound that can be continued by the note without attack.

* If the note without attack is **immediately** after the end of an existing note, it will continue it.
* If the note without attack is shortly after the end of an existing note, while its release is still playing, it will continue it.
* If there are multiple candidate notes that could be continued, it will take the one with the closest matching pitch. This test will consider slides in this calculation (ex: a note without attack being near the end of a slide notes).

## Arpeggio chords

**Arpeggio Chords** take the notes of a chord and arpeggiate it rapidly in a pre-defined sequence. This option is there to mimic a trick often used in chiptune songs where composers would quickly play notes of a chords to make up for the lack of polyphony on old hardware.

To enable arpeggio chords, simply select the notes of a chord, right-click on any selected note (long-press on mobile) and select **Toggle Selection Arpeggio Chords** from the contextual menu. Visually, notes with arpeggio chords enabled will be drawn with a stripe pattern.

> TODO : Image here.

The speed and order in which individual notes of an arpeggio is played is controlled in the channel settings (TODO link + make sure this is documented somewhere). 

> TODO : Image of the channel settings too? Where does that go?

## Release modes

- Explain both release modes

## Ghost notes

# Note Parameters 

## Editing note parameters

## Snapping