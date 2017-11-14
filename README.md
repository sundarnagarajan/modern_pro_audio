
# What is HIFI Audio

I will assume that we share the same understanding of the term 'HIFI audio'. By way of descriptive examples, when I say 'HIFI audio', I think of audio components made by the likes of:
* [Bowers and Wilkins](http://www.bowers-wilkins.com/)
* [Rotel (now part of Bowers and Wilkins)](http://rotel.com/music-systems)[Example Rotel RA 1592](http://rotel.com/product/ra-1592)
* [NAD](http://nadelectronics.com)[Example: NAD C388](http://nadelectronics.com/product/c-388-hybrid-digital-dac-amplifier/)
* [Parasound](http://www.parasound.com/)

HIFI Audio for the purposes of this email will mean something like the term 'prosumer', which is a hybrid category between 'professional' and 'consumer'.

# What do I mean by 'modern'?

## Sources

* Sources are increasingly (and mostly) DIGITAL
    * May be 'lossy' (e.g. MP3, OGG) or 'lossless' (e.g. FLAC, WAV)
    * Transported on [Toslink (S/PDIF)](https://en.wikipedia.org/wiki/S/PDIF​) optical or digital coaxial cables
* Musical pieces (songs) are accessed in 'random access' mode rather than serially
    * Musical pieces (songs) are often (usually) stored in digital form on a filesystem
    * Musical pieces can be 'wound' forwards and backwards by arbitrary amounts also using 'random access'
* Musical pieces (songs) often contain metadata such as Track title, Artist, Album and modern music players look for such metadata (called tags) and often display them
* Younger users (sometimes called 'millenials') exhibit a strong preference for 'streaming music', such as Spotify, Pandora, Soundcloud, Apple Music, Google Music
* Use of Bluetooth (at least as an input source) is quite popular
    * Although (even with the aptX or HDAudio codecs), Bluetooth is probably not HIFI-grade, it is a flexible and popular way to connect
    * Next-gen users (often called 'millenials) like to stream music from their smartphones
    * Bluetooth may be as good as connecting the headset output of a smartphone?

## User interface

* Modern audio equipment (and the users of such equipment) expect a more elaborate and richer user interface - which can include:
    * Larger richer display which may be capable of displaying digital pictures in addition to text
    * Possibly a touch interface - perhaps in addition to traditional buttons
    * Possibly the ability to program the behavior of some or all the physical buttons
* Modern audio equipment should support being controlled through a software interface (API)​
    * This could be in the form of a smartphone application.
    * It could also be through an API exposed over (for example) HTTP or HTTPS.
    * The API is intended to allow control of the equipment
        * Without knowledge of the internal design of the unit being controlled
        * By third parties (other than manufacturer or owner/buyer)
        * By any of a wide class of software programs using public standards - not requiring the participation or approval of the manufacturer
* Event-Function Programmable (EFP): A (relatively) easy way to specify a set of rules of the form: 'when A happens, do B'. Some examples:
    * When it is 06:00 AM, play this song (e.g. alarm clock)
    * When music has been playing for 60 mins without any user input, stop the music and turn all music components off (e.g. sleep timer)
    * When I press button A or call this software API, do the following in sequence:
        * Turn on my power amplifier if it is off
        * Select Toslink_1 as input (Squeezebox)
        * Select Balanced_1 as output
    * When I press SourceUp button, iterate forward through list of available sources
    * When I press OutputUp button, iterate forward through list of outputs
    * When I press Button_Off, do the following:
        * Reduce output volume to SANE_DECIBELS
        * Switch off my power amplifier it if is on
        * Turn off the user interface display
        * Switch computer module to low power mode

# Some rants (complaints) about existing 'ProAudio' audio components

# Key goals and problems to be solved

# Other people who are thinking and working on similar things

# Links

## Class D power amplifiers

## Class T power amplifiers

## Switching mode power supplies

## Ultra-low distortion power amplifiers

## [Balanced audio](https://en.wikipedia.org/wiki/Balanced_audio)




