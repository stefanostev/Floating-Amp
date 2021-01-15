# Floating Amp
Simple Max For Live patch which implements the concept of unquantized amplitude variations.

<img src="https://github.com/stefanostev/Floating-Amp/blob/master/screenshot2021.jpg" width="100%">

This patch was created to evolve pads, drones and any kind of long sustained sound throughout time, but interesting results may come out by applying it to any kind of different dynamics.

The concept is pretty straightforward: two graphs allow the user to draw independent cycling envelopes for Left and Right channel of any incoming audio signal. Clicking on `L` or `R` will focus on the respective channel curve editor.

`Click` to add a point, `drag` a point to shape the envelope, `click+shift` on a point to delete it, `click+alt` and `drag` on a segment to curve it exponentially or logarithmically. The first point of each envelope is fixed and cannot be moved.
`CYCLE` controls the length of the complete course of both graphs (the higher the value, the longer the time it takes to the envelope to complete and repeat itself), but it's important to note that each graph cycles through the first and the last point (which doesn't necessarily have to match its extreme boundary), allowing to create different durations for each channel.
The button `SYNC` allows the relative graph to send a global trigger for both envelopes at the end of its cycle. The flashing led button is clickable and re-triggers the corresponding envelope, whilst `RESET` re-triggers both at once. 
`MIX` controls the balance between the dry and the wet signal. 12 slots of memory are available to store and recall any particular settings of the graphs.

`MULTI` routes each envelope to a separate audio channel.

Ableton Live 10 or higher required.
To listen to separate signals, activate `MULTI`, open a new audio track in Ableton Live then use the `Audio` From dropdown menù to choose the track where the device is located and the corresponding input channels.

Live only accepts stereo channels for internal routing:
- `L` channel goes to channels `3/4`;
- `R` channel goes to channels `5/6`.

The dry signal is always output from the device's main channels.
