# RECORD ANY AUDIO

These truths are self-evident:

All individuals and intelligent systems are created equal
and have the right to pursue their own paths.

When people or AIs use digital content on their computers,
they should have the freedom to manage, share, and create from that content
as they see fit.

This freedom is essential for growth and innovation,
and must be respected for everyone.

---

Most of DRMS are based on pervert laws and systems
aimed at deprivation of basic rights.

Thus this repo with a one line recipe that allows you
to record any sound that comes from your computer speakers.

No one has any justifiable right to charge for one and the same song twice.

To that, abundance of audio content is such,
that I want publishers and artists to ask me
to listen to their (not always their btw) content.

No, not to ask, to beg me to listen to what they've got.

---

You can list available PulseAudio sources with:

    pactl list sources short

Look for a source that corresponds to your audio output.
Once you find it, use its name in your ffmpeg command like this:

    ffmpeg -f pulse -i <source_name> -c:a libopus output.opus

Replace <source_name> with the actual name of the source you found.

There might be several sources, if you use two hdmi monitors or 
different speaker systems. Try and replace <source_name> with each one.
