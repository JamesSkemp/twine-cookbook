# "Audio": Harlowe (v2.0)

!!! Information
    This examples uses two additional files, [testpattern.ogg](testpattern.ogg) and [testpattern.wav](testpattern.wav). Both files need to be downloaded and placed in the same folder as the HTML file in order to work as designed.

## Summary

Harlowe does not have direct macro support for audio resources. However, additional JavaScript can be added to work with [audio elements](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/audio) within a story.

Audio elements rely on sources either absolutely or relatively located. An absolute reference starts with HTTP or another protocol; a relative reference describes the location of the resource in relation to the webpage. Because audio files are external resources, they must also be accessed from a remote service, file hosting location, or stored separately with the webpage.

Due to browser differences in licensing, some audio formats are not universally supported. For best results in using audio in Twine, it is recommended to use multiple formats, allowing the browser to choose which one is best supported when first loaded.

## Example

[Download](harlowe_audio_example.html)

## Twee Code

```twee
:: StoryTitle
Audio in Harlowe

:: Start
<audio controls>
  <source src="testpattern.ogg" type="audio/ogg">
  <source src="testpattern.wav" type="audio/wav">
Your browser does not support the audio element.
</audio>

```

[Twee Download](harlowe_audio_twee.txt)
