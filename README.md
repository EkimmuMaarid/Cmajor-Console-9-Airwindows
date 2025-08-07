### the original plug-in console 9 from Airwindows translated to Cmajor for use inside Daw Waveform natively

You can find the source code of the original C++ plugins at the following link [Console9Channel](https://github.com/airwindows/airwindows/tree/master/plugins/WinVST/Console9Channel) [Console9Buss](https://github.com/airwindows/airwindows/tree/master/plugins/WinVST/Console9Buss)

The cmajor language can be studied at the link [cmajor.dev](https://cmajor.dev/)


## Description

Console plug-ins, using the golden ratio principle, encode the audio signal of each track and then, 
after mixing inside the daw, decompresses the signal code back, thereby obtaining console mixing. 
You can get the details of the whole process, as conceived by the author, from him personally, on his own website.
[Console 9](https://www.airwindows.com/console9/)


## How to use

The Cmajor language, as you can see on their website, is designed to simplify plugin development by facilitating the build process.
You can use this code as part of your cmajor projects, but they were written for native use inside Tracktion's daw Waveform, 
which includes native application of patches written in cmajor.
Two files .cmajor and .cmajorpatch should be stored inside the folder of the same name, which in turn should be located in the cmajor folder, 
next to the vst\au folders and so on. Cmajor files in this location are perceived by waveform as valid audio plug-ins, 
while both patch files are at the same time simple text files and source code, respectively.


## Process events

The actions of the original console plug-in and its effect on sound are completely repeated, while preserving the process. 
The difference, apart from functional solutions, lies in the abolition of the functions of volume controls and panoramas with their smoothing. 
The step taken is justified by the fact that it allows you to automate the encoding and decoding process, 
simplifying the ability to edit the code to easily add a number of audio channels.

Since Waveform itself works directly with only the 32-bit signal size, accordingly, only the 32-bit part of the plug-ins was taken, 
which makes the loss of accuracy in the log1p and expm1 commands insignificant, completely overlapping the original dithering formula.

The plug-ins were written by learning the cmajor language, using artificial intelligence, 
trying to preserve the authenticity of the original idea as much as possible.
