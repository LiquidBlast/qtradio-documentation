# Documentation
API documentation for qtradio.moe

Hi there! Welcome to the API documentation for qtradio.moe.

Notice the two different base urls? That's because we have two different APIs (as of desktop v1.2.0): one for getting the stream and stats (externally) and one for executing actions on the desktop client (internally). 

## Base URL
https://qtradio.moe - External

http://127.0.0.1:3939 - Internal

## Endpoints
### External
GET /stream - Returns .ogg audio stream

GET /opus - Returns .opus audio stream (WIP)

GET /mp3 - Returns .mp3 audio stream (WIP)

GET /streamlow - Returns lower quality audio stream at 128kbps (WIP, also fun fact: that's the quality of listen.moe hahayes)

GET /stats - Returns stream stats
### Internal
GET /togglePlayback - Toggles playback (pause/play)

GET /changeVolume?input=<1-100> - Changes volume

More endpoints soon TM

WIP endpoints will most likely be unstable and may crash at any time. Don't use the metadata on any stream apart from the main one, the others are incorrect.
