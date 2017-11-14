
# What is HIFI Audio

I will assume that we share the same understanding of the term 'HIFI audio'. By way of descriptive examples, when I say 'HIFI audio', I think of audio components made by the likes of:
* [Bowers and Wilkins](http://www.bowers-wilkins.com/)
* [Rotel (now part of Bowers and Wilkins)](http://rotel.com/music-systems) - [Example Rotel RA 1592](http://rotel.com/product/ra-1592)
* [NAD](http://nadelectronics.com) - [Example: NAD C388](http://nadelectronics.com/product/c-388-hybrid-digital-dac-amplifier/)
* [Parasound](http://www.parasound.com/)

HIFI Audio for the purposes of this email will mean something like the term 'prosumer', which is a hybrid category between 'professional' and 'consumer'.

## Audio components being considered here (for transformation / inclusion)
* Pre-amplifier
* [DAC (Digital-Analog Converter)](https://en.wikipedia.org/wiki/Digital-to-analog_converter)
* Input switch
* Output switch
* Power amplifier

# Audio components that _MAY_ be included for transformation (nice to have)
* [Analog to Digital Converter (ADC)](https://en.wikipedia.org/wiki/Analog-to-digital_converter)

## Audio components _NOT_ being considered for transformation - may be included as-is
* Speakers
* Phono pre-amplifier
* Microphone input

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

# Things we can keep from existing 'pro-audio'

## [Balanced audio](https://en.wikipedia.org/wiki/Balanced_audio)


# Some rants (complaints) about existing 'ProAudio' audio components

# Key goals and problems to be solved

# Other people who are thinking and working on similar things

# Links

## Class D power amplifiers
* [FXAudio D802](https://www.amazon.com/192KHz-Digital-Remote-Amplifier-silver/dp/B00WU6JU9Y)
    * Better specs [here on shenzhenaudio.com](https://www.shenzhenaudio.com/fx-audio-d802-80w-2-192khz-coaxial-optical-usb-class-d-digital-power-amplifier-remote-control.html)
        * Digital audio receiver: Asahi Kasei Microdevices AKM4113 - see [datasheet](https://www.akm.com/akm/en/file/datasheet/AK4113VF.pdf)
        * USB 2.0 audio controller: [Via VT1630A](https://www.viatech.com/en/silicon/legacy/audio/vt1630a/)
        * Power amplifier: STMicroelectronics STA326 - see [datasheet](http://www.st.com/content/ccc/resource/technical/document/datasheet/36/12/fe/ee/a4/c8/49/80/CD00062804.pdf/files/CD00062804.pdf/jcr:content/translations/en.CD00062804.pdf)
        * STMicroelectronics STA326 uses [Direct Digital Amplification (DDX) by Apogee Technology Inc](http://www.apogeebio.com/ddx/PDFs/AN-14.pdf)

## Switching mode power supplies
* [Hypex SMPS1200 1200W SMPS](https://www.hypex.nl/product/smps1200/10#tab_description) - see [datasheet](https://www.hypex.nl/img/upload/doc/smps/smps1200/Documentation/SMPS1200Axx0_07xx.pdf)
    * Switching frequency: 100 KHz
    * Continuous output: 325W

## Ultra-low distortion power amplifiers
To be included here, these power amplifiers should promise less than 0.002% THD across the audio spectrum (20 Hz to 20 KHz)
* [A MOSFETPowerAmplifier with ErrorCorrection](http://www.cordellaudio.com/papers/MOSFET_Power_Amp.pdf) - paper by Bob Cordell (1984). Bob Cordell runs an [audio design consultancy](http://www.cordellaudio.com/) and has written a book on [Designing Audio Power Amplifiers](https://www.amazon.com/Designing-Audio-Power-Amplifiers-Cordell/dp/007164024X/)
[* NC252MP 2 x 250W RMS power amplifier with integrated switching mode power supply](https://www.hypex.nl/product/nc252mp-oem/76#tab_description) - see [datasheet](https://www.hypex.nl/img/upload/doc/ncore_mp/nc252mp/Documentation/NC252MP_02xx.pdf)
    * At (Rated Power / 2):
        * 0.0015% THD (typical), 0.0024% THD (max)
    * At 1W:
        * THD not measurable (typical), 0.0015% THD (max)
* [Nord One MP NC252 250W Stereo Power Amp](https://www.nordacoustics.co.uk/product-page/nord-one-mp-nc250-stereo-power-amp-in-silver)
* Uses the NC252MP
* Publishes the same THD specs
* Includes RCA (balun) and Balanced (XLR) inputs
* Auto-sensing 100-240V mains input
* 92% power efficiency
