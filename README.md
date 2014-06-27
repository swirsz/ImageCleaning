ImageCleaning
=============
This Image Cleanup Tool written in Visual Studio 2010 and OpenCV version 2.4.6.0 allows a user to load an image, selectively apply 8 different OpenCV filters (5 built-in filters, 3 custom) to the image in varying degrees in real time.  Changes are shown immediately and can be reversed immediately.

Closing the program automatically saves the output as [filename]_.jpg in the same folder as the original.

## Usage

Simply extract ImageCleaning.exe and the four corresponding DLL files into a directory and execute.

* Image processing is applied on the main image every single time a slider bar is moved, not on a preview of the image. For this reason this application works best on small files.

* Moving a slider bar is reversible until moving a different bar. When a second sliding bar is moved, the modifications by the first are made permanent. There is no undo feature.

* Pressing escape or closing the program will automatically save the output as <filename>_.jpg in the same folder as the original file.

## Compiling

Building this project requires Visual Studio 2010 and OpenCV.  OpenCV version 2.4.6.0 was used in the development of this particular project.  In order to build the project, you need to download and extract OpenCV into a directory of your choosing, run the following command from a command prompt, then import the code into a Visual Studio 2010 project and compile a release build.
```
setx -m OPENCV_DIR "<OpenCV directory>\build"
```

## Source

This project was expanded with an enhanced GUI as a [group project which can be found here.](https://github.com/AleksandrRozenman/Comp467Project)  A [paper describing this group project](http://wirsz.com/ImageCleaning.pdf) is also available.
