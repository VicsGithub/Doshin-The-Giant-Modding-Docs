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
### Using BrawlBox/BrawlCrate
Open up BrawlBox or BrawlCrate and click on File, then click on Open. Alternatively, you can do CTRL+O. Then select and open your TPL file. In the tool, the TPL's images will appear as a list on a hierarchy tree on the left. The images will be order as Texture0, Texture1, Texture2 and so on. When selecting an image, it will appear on the left side on the bottom. Above it are it's properties. They can be modified. There are two arrow buttons that control the image's level of detail (LOD). Right click on the image in the tree view and click on Replace (CTRL-R). Select a new image and click on Open. You will be brought to a screen where you can select the new image's format, edit it's MIP levels, edit the image's palletes (only if it's in a Color Indexed (CI) image format), edit it's dimensions and other things. Click on Okay to replace the image. Remember to save the file by doing CTRL+S.
### Using Wii.cs Tools and TplMii
TplMii is more limited when it comes to editing TPL files. It can only convert singular images to TPL files, and only suppports the RGBA8, RGB565 and RGB5A3 texture formats (ordered as High, Moderate and Low Quality). It can also convert TPL files to images.

To convert an image to TPL, click on the small .. button next to the Image textbox and select an image, then click on the big Convert button. You can modify the TPL's resulting filename and path in the Tpl textbox.
