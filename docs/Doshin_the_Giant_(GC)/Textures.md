# Textures
The textures inside Doshin the Giant's filesystem are contained within <code>root/doshin/textures</code> (PAL) or <code>root/Doshin/textures</code> (JP). They are in the TPL file format. Though, this does not include model textures, as they are found in <code>root/doshin/shapes/</code> (PAL) or <code>root/Doshin/shapes/</code> (JP).

## The Texture Format
**TPL** files (**T**exture **P**alette **L**ibrary) are containers for one or more textures. TPL files originally started out as one of the formats in the Nintendo GAMECUBE Character Pipeline SDK, but was later made a standard format. Textures are encoded with the one of the TEX0 microcode formats.

* I4
* I8
* IA4
* IA8
* RGB565
* RGB5A3
* RGBA32/RGBA8
* C4/CI4
* C8/CI8
* C14X2/CI14x2
* CMPR
## Texture List
TBA

## Editing Textures
### Using BrawlBox
TBA
### Using Wii.cs Tools and TplMii
TplMii is more limited when it comes to editing TPL files. It can only convert singular images to TPL files, and only suppports the RGBA8, RGB565 and RGB5A3 texture formats (ordered as High, Moderate and Low Quality). It can also convert TPL files to images.

To convert an image to TPL, click on the small .. button next to the Image textbox and select an image, then click on the big Convert button. You can modify the TPL's resulting filename and path in the Tpl textbox.
