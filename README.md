# MusicOnAStick

Scripts to simplify creating USB thumb drives containing music,
compatible with a Subaru Ascent console.

The goal is to make it simple and quick to take a bunch of playlists
in M3U files (such as those created by iTunes) and create a USB
thumb drive that can be plugged into the USB port on the Subaru
Ascent console and have it work intuitively.

## Intro

My 2020 Subaru can play music from USB drives plugged into the
stereo unit, but there are some limits/quirks in how it behaves:

 * Songs in an "album" are played in alphabetical order, rather
    than in track order.  Songs in playlists, however, are played
    in the order that they are listed.
 * Only certain types of files work: currently it seems that only
    MP3 files are compatible, even though they're somewhat archaic.
 * The stereo software creates its own index of music on each thumb
    drive, which seems to be keyed off the UUID of the file system
    on the drive.  This means that it's often more convenient to
    rebuild a thumb drive from scratch than to modify it; sometimes
    the car doesn't seem to catch all the changes.  (this might
    have been fixed in more recent revs of the firmware, or it might
    be some other bug, but rebuilding the drives was a workaround)

One approach to the first problem is to create a playlist for each
album, and use the playlists and ignore the albums entirely.  This
works, but if you have a large music collection this adds up to a
_lot_ of playlists, and navigating them is not as convenient as
navigating the album lists.  Therefore, it would be really nice to
find a way to fix this.

The second problem is solved by making a copy of the necessary music
files converted to MP3 format, and keep these in a cache so that
we don't have to re-convert the files repeatedly when we completely
recreate a thumb drive.

## State of the software

Nothing works; some things are partly functional.

Stay tuned.

