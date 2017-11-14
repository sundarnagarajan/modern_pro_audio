
# What is HIFI Audio

I will assume that we share the same understanding of the term 'HIFI audio'. By way of descriptive examples, when I say 'HIFI audio', I think of audio components made by the likes of:
* [Bowers and Wilkins](http://www.bowers-wilkins.com/)
* [Rotel (now part of Bowers and Wilkins)](http://rotel.com/music-systems) - [Example Rotel RA 1592](http://rotel.com/product/ra-1592)
* [NAD](http://nadelectronics.com) - [Example: NAD C388](http://nadelectronics.com/product/c-388-hybrid-digital-dac-amplifier/)
* [Parasound](http://www.parasound.com/)
* [McIntosh](http://www.mcintoshlabs.com/us/Products/pages/categorylanding.aspx?CatId=Amplifiers) - [Example McIntosh MC152 2 x 150W](http://www.mcintoshlabs.com/us/Products/pages/ProductDetails.aspx?CatId=amplifiers&ProductId=MC152)

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
    * Home automation use-cases
        * When my home automation system detects I have left home, turn off my audio components if they are on

# Things we can adopt (keep) from existing 'pro-audio'

## [Balanced audio](https://en.wikipedia.org/wiki/Balanced_audio)

Excerpt from wikipedia:

Balanced audio is a method of interconnecting audio equipment using balanced lines. This type of connection is very important in sound recording and production because it allows the use of long cables while reducing susceptibility to external noise caused by electromagnetic interference.
Balanced connections typically use shielded twisted-pair cable and three-conductor connectors. The connectors are usually XLR or TRS phone connectors. When used in this manner, each cable carries one channel, therefore stereo audio (for example) would require two of them.

### [Balanced audio connectors](https://en.wikipedia.org/wiki/Balanced_audio#Connectors)
3-pin XLR connectors and quarter-inch (¼" or 6.35 mm) TRS phone connectors are commonly used for balanced audio signals. Many jacks are now designed to take either XLR or TRS phone plugs. Equipment intended for long-term installation sometimes uses terminal strips or Euroblock connectors.

With XLR connectors, pins 1, 2, and 3 are usually used for the shield (earthed or chassis), the non-inverting signal, and the inverting signal, respectively. (The phrase "ground, live, return", corresponding to "X, L, R", is often offered as a memory aid, although the inverting signal is not simply a "return.") On TRS phone plugs, the tip is non-inverting, the ring is inverting, and the sleeve is ground.

### [Converters](https://en.wikipedia.org/wiki/Balanced_audio#Converters)
Unbalanced signals can be converted to balanced signals by the use of a [balun](https://en.wikipedia.org/wiki/Balun), often through a DI unit (also called a "DI box" or "direct box").
If balanced audio must be fed into an unbalanced connection, the electronic design used for the balanced output stage must be known. In most cases the negative output can be tied to ground, but in certain cases the negative output should be left disconnected

### Converting XLR (Balanced) to RCA (unbalanced)
See [this discussion on audiogon](https://forum.audiogon.com/discussions/is-it-save-to-convert-xlr-to-rca) - it is possible, and easy and will not damage RCA equipment, but (of course) you lose the benefits of balanced XLR. Here is an example of a [stereo (2-channel) XLR Female to RCA  Male cable on Amazon for $10](https://www.amazon.com/dp/B000V1RLI2/) a [stereo XLR Male to RCA Male cable on Amazon for $9.50](https://www.amazon.com/Stagg-STC3CMXM-Male-Twin-Cable/dp/B003SOR6UC)

# Some rants (complaints) about existing 'ProAudio' audio components
## The cost can be absurd!
Some examples - definitely not the most outrageous!
* [Rotel RA-1592 2 x 200W amplifier: $2500](https://www.magnoliaav.com/shop/audio/av-separates/p/rotel-RA-1592-SILVER-5708757)
* [Rotel RA-1570 2 x 120W amplifier: $1600](https://www.magnoliaav.com/shop/audio/av-separates/p/rotel-RA-1570-SILVER-5708760)
* [Rotel RSP-1572 pre-amplifier: $2200](https://www.magnoliaav.com/shop/audio/av-receivers/p/rotel-RSP-1572-SILVER-5708430)
* [NAD C388 2 x 150W power amplifier: $1600](https://www.crutchfield.com/p_745C388/NAD-C-388.html?tp=34948&awkw=262153781688&awat=pla&awnw=g&awcr=147307116170&awdv=c&awug=9032020)
* [Anthem Integrated 2 x 400W amplifier: $4500](https://www.anthemav.com/products-current/model=str-integrated-amplifier/page=specs)
* [Peachtree Audio nova150 2 x 150W Class D amplifier: $1500](https://www.peachtreeaudio.com/nova150-amplifier-with-dac.html)
* [Peachtree Audio nova300 2 x 300W Class D amplifier: $2000](https://www.peachtreeaudio.com/nova300-amplifier-with-dac.html)
* [McIntosh MC152 2 x 150W amplifier: $4500](https://www.crutchfield.com/p_958MC152/McIntosh-MC152.html?tp=180&awcp=1t1&awcr=196735223404&awdv=c&awkw=%2bmcintosh+%2bmc152&awmt=b&awnw=g&awug=9032020)
* [McIntosh MC301 **Monoblock** 1x300W: $5000](https://www.crutchfield.com/p_958MC301/McIntosh-MC301.html)
* [McIntosh MA5300 2 x 100W amplifier with DAC: $5000](https://www.crutchfield.com/p_958MA5300/McIntosh-MA5300.html)
* [NAD C 275BEE 2 x 150W power amplifier: $1300](https://www.crutchfield.com/p_745C275BEE/NAD-C-275BEE.html?tp=180&awkw=75620915785&awat=pla&awnw=g&awcr=47439361105&awdv=c&awug=9032020)
* [Arcam A49 2 x 200W amplifier: $5750](http://www.audiolab.com/arcam-a49-audiophile-stereo-integrated-amplifier)
* [Roksan Blak Integrated USB 2 x 230W amplifier: $5000](http://www.rutherfordaudio.com/introducing-new-blak-series-roksan/)
* [Audio Research GSi75 2 x 75W amplifier: $10695](https://www.paragonsns.com/product/audio-research-gsi75-integrated-amplifier/)

## Do not provide schematics (any more)
## Lack of 'modern' perspective
* IR remote control is the only interface provided other than physical buttons
* Software API is almost unheard of, although Rotel does publish some their [RS232 protocol](http://rotel.com/sites/default/files/product/rs232/RA1592%20Protocol.pdf) and the [IR Hex codes for their remote control](http://rotel.com/sites/default/files/product/ir/RA1592%20HEX.pdf)
* Display customization is impossible - not even considered
* Creating 'activities' and macros (sequences of operations for connecting components together to perform an activity like 'Listen to Squeezebox') is left to third parties like [Logitech](https://secure.logitech.com/en-us/product/harmony-hub), [Blumoo](http://www.blumoo.com/) or [Pronto](https://www.amazon.com/Pronto-Universal-Control-Compatible-Android/dp/B00Y2SIYP4). These devices invariably try to bridge between Bluetooth and IR, and invariably do not have an open API

# Key goals and problems to be solved

# Other people who are thinking and working on similar things

# Links

## Classes of amplifiers
* [Audio Amplifier Classes (A, A/B, D, G, and H): What are the Differences?](http://www.audioholics.com/audio-amplifier/amplifier-classes)


## Class D power amplifiers
* [FXAudio D802 2 x 80W Digital amplifier: $110](https://www.amazon.com/192KHz-Digital-Remote-Amplifier-silver/dp/B00WU6JU9Y)
    * Better specs [here on shenzhenaudio.com](https://www.shenzhenaudio.com/fx-audio-d802-80w-2-192khz-coaxial-optical-usb-class-d-digital-power-amplifier-remote-control.html)
        * Digital audio receiver: Asahi Kasei Microdevices AKM4113 - see [datasheet](https://www.akm.com/akm/en/file/datasheet/AK4113VF.pdf)
        * USB 2.0 audio controller: [Via VT1630A](https://www.viatech.com/en/silicon/legacy/audio/vt1630a/)
        * Power amplifier: STMicroelectronics STA326 - see [datasheet](http://www.st.com/content/ccc/resource/technical/document/datasheet/36/12/fe/ee/a4/c8/49/80/CD00062804.pdf/files/CD00062804.pdf/jcr:content/translations/en.CD00062804.pdf)
        * STMicroelectronics STA326 uses [Direct Digital Amplification (DDX) by Apogee Technology Inc](http://www.apogeebio.com/ddx/PDFs/AN-14.pdf)
* [SMSL Q5 Pro 2 x 50W Digital Amplifier: $140](https://www.amazon.com/dp/B017W12UCU)
    * Available [cheaper ($115) here](https://www.parts-express.com/smsl-q5-pro-stereo-amplifier-usb-optical-coaxial-dac-with-subwoofer-output-2x40w--230-210)
* [Review of 4 class D amplifiers, including the FXAudio D802](http://www.qobuz.com/ie-en/info/hi-res-guide/comparison-four-digital-amplifiers178041)
* [STA326 aliexpress.com search](https://www.aliexpress.com/wholesale?catId=0&initiative_id=SB_20171113195149&SearchText=STA326)
* [STA326 eBay search](https://www.ebay.com/sch/i.html?_from=R40&_sacat=0&_nkw=STA326+amplifier&rt=nc&LH_BIN=1)


## Class T Power amplifiers
* [ALIENTEK D8 2 x 80W Class T digital amplifier: $85](https://www.aliexpress.com/item/ALIENTEK-D8-SMSL-Pro-Pure-Digital-HiFi-Amplifier-USB-Fiber-Coaxial-Optical-Audio-Power-PCM2704/32585939013.html?spm=2114.12010108.1000013.10.48692492bhPzXy&traffic_analysisId=recommend_2088_5_90158_iswistore&scm=1007.13339.90158.0&pvid=064f3d83-d8c0-4e87-ad88-761132882a25&tpp=1)
    * Available on [Amazon for $126 through third-party selelrs](https://www.amazon.com/XMOS-ALIENTEK-Amplifier-Headphone-Supply-Black/dp/B075L21N8X)
    * PCM7204 (DAC?)
    * STA328 Class D amplifier - [datasheet](http://www.st.com/content/ccc/resource/technical/document/datasheet/36/92/fb/cf/e4/11/49/f2/CD00043329.pdf/files/CD00043329.pdf/jcr:content/translations/en.CD00043329.pdf)
    * PCM1522
    * [Asahi Kasei Microdevices AK5358 4-channel DAC](https://www.akm.com/akm/en/file/datasheet/AK5388AEQ.pdf)
    * [Cirrus Logic WM8805 S/PDIF transceiver](https://www.cirrus.com/products/wm8805/)
* [Dayton Audio DTA-120 Class T 2 x 60W Amplifier: $88](https://www.amazon.com/Dayton-Audio-DTA-120-Digital-Amplifier/dp/B00HFG3FYA)
    * No digital inputs
* [Lepy LP-2051 2 x 50W Class T amplifier: $46](https://www.amazon.com/Lepy-LP-2051-Hi-Fi-Amplifier-Stereo/dp/B01M6BMKD6)
    * Uses  LP-2051 Audio Amplifier IC
    * No digital inputs
* [Topping TP32EX 2 x 50W Class T Amplifier: $120](https://www.amazon.com/Topping-Amplifier-Coaxial-Digital-Headphone/dp/B071RJGQZW)
    * Uses TK2050
    * [Cirrus Logic CS3310 Stereo Digital Volume Control](https://www.cirrus.com/products/cs3310/)

## Class D amplifier boards
* [TPA3116 D2 2 x 120W with bluetooth: $14](https://www.ebay.com/itm/TPA3116-D2-120W-120W-Dual-Channel-Bluetooth-digital-Power-Audio-Amplifier-Board/172795704784?_trkparms=aid%3D555018%26algo%3DPL.SIM%26ao%3D2%26asc%3D41375%26meid%3Db62847df3842421b91d87778894f7d26%26pid%3D100005%26rk%3D1%26rkt%3D6%26sd%3D232530115860&_trksid=p2047675.c100005.m1851)
    * Uses TPA3116 D2 - [datasheet](http://www.ti.com/lit/ds/symlink/tpa3116d2.pdf)
    * 120W is probably PEAK output, since TPA3116D2 is rated by TI at 2 x 50W
    * Needs mains AC-to-DC 24V 10A SMPS
    * [eBay search for TPA3116D2](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2047675.m570.l1313.TR1.TRC0.A0.H0.XTPA3116D2120W.TRS0&_nkw=TPA3116D2120W&_sacat=0)

## Switching mode power supplies
* [Hypex SMPS1200 1200W SMPS](https://www.hypex.nl/product/smps1200/10#tab_description) - see [datasheet](https://www.hypex.nl/img/upload/doc/smps/smps1200/Documentation/SMPS1200Axx0_07xx.pdf)
    * Switching frequency: 100 KHz
    * Continuous output: 325W
 * [Discussion on electronics.stackexahange.com on using SMPS for audio circuits](https://electronics.stackexchange.com/questions/36674/can-an-audio-circuit-be-powered-by-a-switched-mode-power-supply)
 * [Mains AC-to-DC 24V 10A SMPS eBay search](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2047675.m570.l1312.R1.TR0.TRC0.A0.H1.TRS5&_nkw=AC+to+DC+24V+10A+switching+power+supply&_sacat=0)
 * [Kasonic universal AC-to-DC 24V 10A SMPS: $15](https://www.ebay.com/itm/Kasonic-Universal-12V-24V-DC-Power-Supply-Driver-Adapter-For-LED-Strip/152483355211)
 * [Mains AC-to-DC 36V 5A SMPS eBay search](https://www.ebay.com/sch/i.html?_odkw=AC+to+DC+32V+5A+switching+power+supply&_osacat=0&_from=R40&_trksid=p2045573.m570.l1313.TR0.TRC0.H0.XAC+to+DC+3V+5A+switching+power+supply.TRS0&_nkw=AC+to+DC+36V+5A+switching+power+supply&_sacat=0)

## DIY Audio links
* [diyaudio.com](http://www.diyaudio.com/)
* [AMB Laboratories](https://www.amb.org/audio/)
* [Yuan Jing Audio](https://www.yuan-jing.com/)

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

# Other informative links
* [AV Receiver and Amplifier Power Ratings Trends: Manipulating Wattage Ratings (Audioholics)](http://www.audioholics.com/audio-amplifier/product-managing-receiver-platforms-power-ratings)
* [The All Channels Driven (ACD) Amplifier Test (Audioholics)](http://www.audioholics.com/audio-amplifier/the-all-channels-driven-acd-amplifier-test)
* [The All Channels Driven Amplifier Test Controversy (audioholics)](http://www.audioholics.com/audio-amplifier/the-all-channels-driven-amplifier-test-controversy)

