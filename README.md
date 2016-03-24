GUI
===
This is a "simple" example of how to create an OpenGL application on Windows,
Mac OS X and Linux that correctly deals with...
* Alt-Tabbing
* Multiple Monitors
* Xbox Controllers
* Icons
* Changing to and from fullscreen


Build Environment
=================
Windows
-------
* Install [mingw-w64-install.exe](http://sourceforge.net/projects/mingw-w64/files/)
* Install http://msysgit.github.io/
* Put their ``/bin`` directories in your ``PATH``.
* Install [ImageMagick](http://www.imagemagick.org/script/binary-releases.php#windows)

Mac OS X Yosemite
-----------------
* Install [XCode](https://developer.apple.com/xcode/downloads/)

Debian & Ubuntu
---------------
    sudo apt-get install a56 imagemagick git-core libglu1-mesa-dev libxi-dev ocl-icd-opencl-dev mingw-w64 
If cross compiling, copy the OpenCL library and headers from the Windows setup to ``/usr/x86_64-w64-mingw32/``

Build Instructions
------------------
    git clone git@github.com:burito/opengl.git		# if you're using ssh
    cd opengl
    make -j8		# if you have 8 threads

By default, it will build the binary native for your platform.

    make gui		# builds the default linux binary
    make gui.exe	# builds the default windows binary
    make gui.app	# builds the default OSX binary

Usage
-----
* ESC quits.
* F11 Toggles Fullscreen.

Please refer to the articles at...

http://danpburke.blogspot.com.au

...for the complete set of ramblings.

