# Floating-Amp
Simple Max For Live patch which implements the concept of unquantized amplitude variations.


This patch was created to evolve pads, drones and any kind of long sustained sound throughout time, but interesting results may come out of applying it to any kind of different dynamics.

The concept is pretty basic but powerful: two graphs allow the user to draw independent cycling envelopes for Left and Right channel of any incoming audio signal: click to add a point, drag a point to shape the envelope, click+shift on a point to delete it. `CYCLE` controls the length of the complete course of both graphs (the higher the value, the longer the time it takes to the envelope to complete and repeat itself), but it's important to note that each graph cycles through the first and the last point (which don't necessarily have to match its extreme boundaries), allowing to create different durations for each channel. The button `SYNC` allows the relative graph to send a global trigger for both envelopes at the end of its cycle, essentially syncing the starting point of both, which might be very useful when working with envelopes of different lengths. `START` re-triggers the correspondent envelope, whilst `RESET` re-triggers both at once. `MIX` controls the balance between the dry and the wet signal. 12 slots of memory are available to store and recall any particular settings of the graphs.


The "multi-outputs" version has an additional toggle button `MULTI` which allows audio routing of individual channels to separate tracks.

For this version is required Ableton Live 10 or higher.
To listen to separate signals, activate `MULTI`, open a new audio track in Ableton Live then use the Audio From dropdown menù to choose the track where the device is located and the corresponding input channels.

Live only accepts stereo channels for internal routing:
- L channel goes to channels 3/4;
- R channel goes to channels 5/6.

The dry signal is always output from the device's main channels.
