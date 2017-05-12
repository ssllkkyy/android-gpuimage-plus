# Android-GPUImage-Plus
Image, Camera And Video Filters Based On OpenGL.

## Abstract ##

1.  This repo is an "Android Studio Project", comprising "cgeDemo", "library" two sub-modules. All java code and the "libCGE.so"(Written in C++&OpenGL with NDK) is provided. Hundreds of built-in filters are available in the demo. 😋If you'd like to add your own filter, please take a look at the manual page.
(Ch: 本repo为一个Android Studio Project, 包含 cgeDemo, library 两个子模块. 其中library 模块包含java部分所有代码以及一个包含cge核心模块的so链接库，内置近百种滤镜效果， 😋如果要自行添加滤镜， 请参考下方的文档页面。)

2. Demo and Library will be updated as needed. Welcome for your questions or PR.
(Ch: 不定期更新demo和library. 如有问题欢迎提问， 也欢迎PR.)

3. iOS version: [https://github.com/wysaid/ios-gpuimage-plus](https://github.com/wysaid/ios-gpuimage-plus "http://wysaid.org")

4. Extra functions can be provided to the donors such as 'realtime video recording with gpu filters'. See the precompiled apk about this function: [https://github.com/wysaid/android-gpuimage-plus/tree/master/demoRelease](https://github.com/wysaid/android-gpuimage-plus/tree/master/demoRelease "http://wysaid.org")

5. To build with the jni part, pleasae try: (The precompiled '.so' files are using NDK-r10e, and the newest version NDK-r13b(3/17/2017) is also supported.)
```
export NDK=path/of/your/ndk
cd folder/of/jni (android-gpuimage-plus/library/src/main/jni)

#This will make all arch: armeabi, armeabi-v7a arm64-v8a, x86
./buildJNI

#Try this if you failed to run the shell above
export CGE_USE_VIDEO_MODULE=1
$NDK/ndk-build
```
Note that the generated file "libFaceTracker.so" is not necessary. So just remove this file if you don't want any feature of it.

## Manual ##

En: [https://github.com/wysaid/android-gpuimage-plus/wiki/Parsing-String-Rule-En](https://github.com/wysaid/android-gpuimage-plus/wiki/Parsing-String-Rule-En "http://wysaid.org")

Ch: [https://github.com/wysaid/android-gpuimage-plus/wiki/Parsing-String-Rule](https://github.com/wysaid/android-gpuimage-plus/wiki/Parsing-String-Rule "http://wysaid.org")

>Note: you can add your own shader filter with c++. Please see the demo for further details.

## Tool ##

Some utils are available for new version: [https://github.com/wysaid/cge-tools](https://github.com/wysaid/cge-tools "http://wysaid.org")

[![Tool](https://raw.githubusercontent.com/wysaid/cge-tools/master/screenshots/0.jpg "cge-tool")](https://github.com/wysaid/cge-tools)

## Donate ##

Alipay:

![Alipay](https://raw.githubusercontent.com/wysaid/android-gpuimage-plus/master/screenshots/alipay.jpg "alipay")

Paypal: 

[![Paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif "Paypal")](http://blog.wysaid.org/p/donate.html)
