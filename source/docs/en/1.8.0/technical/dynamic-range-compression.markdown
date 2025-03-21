---
Type:            article
State:           [ obsolete ]
Title:           Dynamic Range Compression
Project:         HandBrake
Project_URL:     https://handbrake.fr/
Project_Version: 1.8.0
Language:        English
Language_Code:   en
Authors:         [ Scott (s55) ]
Copyright:       2024 HandBrake Team
License:         Creative Commons Attribution-ShareAlike 4.0 International
License_Abbr:    CC BY-SA 4.0
License_URL:     https://handbrake.fr/docs/license.html
---

Dynamic Range Compression
=============================

The dynamic range of an audio track is the difference between the softest and loudest sounds.

Dynamic range compression reduces the gap between those extremes.

- 1.0-2.5 are good values to use.
- 0, the default, turns it off completely.
- 1.0 uses the compression hints embedded in the AC3 track.
- Values greater than 1.0 compress the range further by boosting the volume of soft sound samples while leaving loud samples as they are. This squeezes down the range between the softest and loudest parts, but should make the softer ones easier to hear in noisy listening environments.

Note, this is not the same as a gain or volume boost control.

### Compatibility

Dynamic range compression only works when the source audio is AC3 and you are encoding to another format, like AAC. It has no effect on AC3 pass-through or on DTS or MPEG-2 audio.