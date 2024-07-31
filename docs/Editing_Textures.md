# Textures
The game's textures are found in `doshin/textures/` (PAL) or `Doshin/textures/` (JP). The textures for the game's models however, are found in `doshin/shapes/(model name)/` (PAL) or `Doshin/shapes/(model name)/` and they share the name of their respective model.

# The Texture Format
All of the game's textures are in the TPL file format. **TPL** files (**T**exture **P**alette **L**ibrary) files are containers for one or more images. originally started out as one of the formats in the Nintendo GAMECUBE Character Pipeline SDK, but later spun off as a common GameCube file format used in various games.

## File Format
A TPL file consists of:
* File header
* Image offset table
* One or more images

Each image contains:
* A palette header (optional)
* Palette data (optional)
* An image header
* Image data

### Header
TBA

### Image Offset Table
TBA

### Palette Header
TBA

### Image Header
TBA
#### Image Formats
| ID | Name | Bits per pixel | Block width | Block height | Block size | Type |
| --- | --- | --- | --- | --- | --- | --- |
| 0x00 | I4 | 4 | 8 | 8 | 32 bytes | Gray |
| 0x01 | I8 | 8 | 8 | 4 | 32 bytes | Gray |
| 0x02 | IA4 | 8 | 8 | 4 | 32 bytes | Gray + Alpha |
| 0x03 | IA8 | 16 | 4 | 4 | 32 bytes | Gray + Alpha |
| 0x04 | RGB565 | 16 | 4 | 4 | 32 bytes | Color |
| 0x05 | RGB5A3 | 16 | 4 | 4 | 32 bytes | Color + Alpha |
| 0x06 | RGBA32 (RGBA8) | 32 | 4 | 4 | 64 bytes | Color + Alpha |
| 0x08 | C4 (CI4) | 4 | 8 | 8 | 32 bytes | Palette (IA8, RGB565, RGB5A3) |
| 0x09 | C8 (CI8) | 8 | 8 | 4 | 32 bytes | Palette (IA8, RGB565, RGB5A3) |
| 0x0A | C14X2 (CI14x2) | 16 | 4 | 4 | 32 bytes | Palette (IA8, RGB565, RGB5A3) |
| 0x0E | CMPR | 4 | 8 | 8 | 32 bytes | Color + optional Alpha (compressed) |

### Image
TBA

# Editing TPL Files using BrawlBox
If you haven't downloaded BrawlBox, download it [here](https://github.com/libertyernie/brawltools/releases/download/v0.78_h1/BrawlBox.v0.78.Hotfix.1.exe).

Open up BrawlBox and click on File, then click on Open. Alternatively, you can do CTRL+O. Then select and open your TPL file. In BrawlBox, the TPL's images will appear as a list on a hierarchy tree on the left. The images will be order as Texture0, Texture1, Texture2 and so on. When selecting an image, it will appear on the left side on the bottom. Above it are it's properties. They can be modified. There are two arrow buttons that control the image's level of detail (LOD). Right click on the image in the tree view and click on Replace (CTRL-R). Select a new image and click on Open. You will be brought to a screen where you can select the new image's format, edit it's MIP levels, edit the image's palletes (only if it's in a Color Indexed (CI) image format), edit it's dimensions and other things. Click on Okay to replace the image. Remember to save the file by doing CTRL+S.
