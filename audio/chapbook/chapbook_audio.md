# "Adding Functionality": Chapbook (v1.0.0)

## Summary

Chapbook supports both looping sounds (which it calls ambient) and one-off sound
(which it calls effects). It only allows playing one ambient sound at a time.
Please see the [Audio] section of the [Chapbook Guide] for details on how these
work.

<div class="alertbox information"><strong>Note:</strong> This examples uses two additional files, <a href="testpattern.ogg">testpattern.ogg</a> and <a href="testpattern.wav">testpattern.wav</a>. Both files need to be downloaded and placed in the same folder as the HTML file in order to work as designed.</div>

## Live Example

<section>
<iframe src="chapbook_adding_functionality_example.html" height=400 width=90%></iframe>


Download: <a href="chapbook_adding_functionality_example.html" target="_blank">Live Example</a>
</section>

## Twee Code

```
:: Start
sound.ambient.test.url: 'testpattern.ogg'
sound.ambient.test.description: 'An audio test pattern'
--

> [[Play sound]]
> [[Stop the sound]] 

:: Play sound
{ambient sound: 'test'}

[[Return->Start]]

:: Stop the sound
sound.ambient.test.playing: false
--

[[Return->Start]]
```

[Audio]: https://klembot.github.io/chapbook/guide/multimedia/audio.html
[Chapbook Guide]: https://klembot.github.io/chapbook/guide