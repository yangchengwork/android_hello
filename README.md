android_hello
=============

使用NDK编译可以执行的Hello world

编译时先安装NDK，安装好后，依照真实目录修改Makefile.android中的NDK_ROOT和ANDROID_NDK，下面是我电脑上的目录。
NDK_ROOT=/home/gump/work/android-ndk-linux
ANDROID_NDK = /home/gump/work/android-ndk-linux
修改后执行
make -f Makefile.android就可以生成test执行文件，在push到真实机器上通过串口，或adb shell cat /proc/kmsg可以看到信息。
注意这一步需要root
