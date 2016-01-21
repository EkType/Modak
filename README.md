# **Modak**

Modak is a sweet plump Devanagari+Latin display typeface with portly curves and thin counters. It is Unicode compliant and is open sourced under the SIL Open Font License v1.1.

It began as a heavy hand-sketched letterform exploration in Devanagari with cute, adorable characters whose curves merged into each other, forming distinct counter shapes.  As we translated these into a functional font, each character was fine-tuned and multiple matras designed to match precisely with every character. Unlike the conventional approach the post-base matras in Modak overlap the consonants. Likewise overlapping ukars were also designed leaving thin counters in between. Rather than being a mere composite of 2 separate glyphs, every conjunct was redrawn as a single entity. The challenge was to maintain legibility and consistency in the thin counter spaces across all characters, irrespective of their structural complexity. The resulting typeface is one of its kind and most likely the chubbiest Devanagari typeface to be designed so far.

Modak Devanagari is designed by Sarang Kulkarni and Maithili Shingre and Modak Latin by Noopur Datye with support from Girish Dalvi. This project is led by [Ek Type]( http://ektype.in/), a collective of type designers based in Mumbai focused on designing contemporary Indian typefaces.

We are immensely thankful to Santosh Kshirsagar, Pradnya Naik, Yashodeep Gholap and Dave Crossland for their suggestions and feedback during the font design process. We are also grateful to our friends from the Industrial Design Centre, IIT Bombay and Sir J J Institute of Applied Art for their support and encouragement.


## License

Modak is licensed under the SIL Open Font License v1.1 (<http://scripts.sil.org/OFL>). To view the copyright and specific terms and conditions please refer to [OFL.txt](https://github.com/girish-dalvi/Modak/blob/master/OFL.txt)


## Downloading font binaries (TTF files)

Find binary releases on <https://github.com/girish-dalvi/Modak/releases>

## How do I install the font on my computer?

First download the font binaries (TTF files) from the master branch, then follow the instructions given below.

- [Windows](http://windows.microsoft.com/en-us/windows-vista/install-or-uninstall-fonts)

- [GNU/Linux](http://lmgtfy.com/?q=how+to+install+fonts+in+linux)

- [Mac OS X](http://support.apple.com/kb/HT2509)

## Getting Involved

Would you like to contribute to the development of this font? Here is how **you** can help:

1. Tell us about any bugs you find, or enhancements you would like to see

2. Contribute directly to the fonts. In this repository we provide the complete set of source files that we use ourselves to develop the fonts. If you with to contribute directly, please see below how we build the fonts and follow our build process so that we can easily include your contribution, and follow the Github pull request process to send your contribution. 

### Bug Reports

Send us bug reports, feature enhancements or glyph requests, using the [Github Issue Tracker](https://github.com/girish-dalvi/Modak/issues/). Here are a few tips:

- Bugs must be isolated and reproducible problems that we can fix. This means telling us step by step how we can produce the bug.
- Share as much information as possible. Include your operating system and its version, what application(s) you found the problem with and their version, etc. 

## Building the font from source
   
This requires the following programs:

- **[Fontlab Studio](http://www.fontlab.com/font-editor/fontlab-studio/):** `.vfb` design files are used by this font editor, for Windows and Mac from the Fontlab company with a proprietary license and requiring a license fee from each user. 

- **[AFDKO](http://www.adobe.com/devnet/opentype/afdko.html):** A set of command line tools for generating OpenType fonts from Adobe


The build process used by Ek Type is as follows:

1. Make changes in FontLab `.vfb` file

2. Generate the `.ttf` file

3. Make changes in AFDKO feature files. 

4. Type the following commands in the Command prompt window. Make sure that the AFDKO directory is included in your path.

`tx -t1 Modak.ttf > Modak.pfa`

This will convert the `.ttf`  font to a `.pfa` font.

Use `maketof -h` to view the options available to you; choose the options you want as per your needs. We generally use  
`makeotf -f Modak.pfa -o Modak.otf -r -S -shw -ga -gs -rev`

to generate the release version of the font. 

### Branches and Pull Requests

To learn more about Pull Requests, see Github's great article on [using pull requests](https://help.github.com/articles/using-pull-requests) and play the [interactive learning game](http://try.github.com) that takes around 15 minutes to complete.

- `master` is the latest, stable, tested version 

- Add your name to the contributors file

- Explain in the pull request how you have tested your contribution
