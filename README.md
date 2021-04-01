# bulk2x-ncnn-vulkan
Simple GUI to make it easy to use [waifu2x-ncnn-vulkan](https://github.com/nihui/waifu2x-ncnn-vulkan) with individual files and whole directories.

![screenshot_0.png](.screenshots/screenshot_0.png)

# Dependencies
 - [Python 3](https://www.python.org/downloads/)
 - [PyGObject](https://pypi.org/project/PyGObject/)
 - [GTK 3](https://www.gtk.org/)
 - [waifu2x-ncnn-vulkan](https://github.com/nihui/waifu2x-ncnn-vulkan) (or [wget](https://www.gnu.org/software/wget/wget.html) and [unzip](http://infozip.sourceforge.net/UnZip.html))

# Obtaining
You can download a compressed archive ([zip](https://gitlab.com/nickgirga/bulk2x-ncnn-vulkan/-/archive/master/bulk2x-ncnn-vulkan-master.zip), [tar.gz](https://gitlab.com/nickgirga/bulk2x-ncnn-vulkan/-/archive/master/bulk2x-ncnn-vulkan-master.tar.gz), [tar.bz2](https://gitlab.com/nickgirga/bulk2x-ncnn-vulkan/-/archive/master/bulk2x-ncnn-vulkan-master.tar.bz2), [tar](https://gitlab.com/nickgirga/bulk2x-ncnn-vulkan/-/archive/master/bulk2x-ncnn-vulkan-master.tar)) of the repository from the [project overview](https://gitlab.com/nickgirga/bulk2x-ncnn-vulkan) or you can clone the repository using git by running `git clone https://gitlab.com/nickgirga/bulk2x-ncnn-vulkan.git`. If you downloaded a compressed archive, decompress it using the appropriate tool (unzip, tar). Then head to the [running](#running) section.

# Running
Make sure you have all of the [dependencies](#dependencies) installed. Then, simply run `./bulk2x-ncnn-vulkan` in the root directory of the repository. If you do not have [waifu2x-ncnn-vulkan](https://github.com/nihui/waifu2x-ncnn-vulkan) installed, bulk2x-ncnn-vulkan will download [Release 20210210](https://github.com/nihui/waifu2x-ncnn-vulkan/releases/tag/20210210) and unzip it for you. If your system does not support interpreting foreign files with third-party interpreters like python using a shebang, you can run `python3 bulk2x-ncnn-vulkan`. However this will only work if `python3` is a command that is accessible from anywhere. If your environment does not support this, add the path to your `python3` binary before it, but continue to run the command within the root folder of the repository. This script requires resources such as the glade file, so running it from any other folder will likely result in an error.
