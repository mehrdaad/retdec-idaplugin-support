# RetDec IDA Plugin Support

Support packages for the [RetDec IDA plugin](https://github.com/avast-tl/retdec-idaplugin).

Packages contain prebuilt libraries needed tu build RetDec IDA plugin. The following packages are available:
* [Arch Linux gcc-5.2](https://github.com/avast-tl/retdec-idaplugin-support/releases/download/2017-12-14/retdec-idaplugin-libs-2017-12-14-arch-linux-gcc52.zip)
* [Debian Linux gcc-4.9](https://github.com/avast-tl/retdec-idaplugin-support/releases/download/2017-12-14/retdec-idaplugin-libs-2017-12-14-debian-linux-gcc49.zip)
* [Windows Visual Studio 2015](https://github.com/avast-tl/retdec-idaplugin-support/releases/download/2017-12-14/retdec-idaplugin-libs-2017-12-14-windows-msvc2015.zip)

You can try to use these packages even if you are not running an exact combination of operating system and compiler. It often works, but nothing is guaranteed. If the build fails, or the resulting plugin does not work, you need to build the support libraries on your own, or by using `download-and-build-libs.sh` as described in the RetDec IDA plugin [repository](https://github.com/avast-tl/retdec-idaplugin#requirements).

## Use

* Download and extract an applicable package.
* When configuring `cmake` during the RetDec IDA plugin build, set `<path>` in `-DIDAPLUGIN_LIBS_DIR=<path>` to an absolute path to the extracted directory.

## Status

This is a temporary solution. It would be the best if the required libraries were automatically downloaded and built during the RetDec IDA plugin build. Once this is done, this repository will not be needed anymore.
