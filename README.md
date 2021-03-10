# spdlog4iosbuild

$ cd spdlog-1.8.2
$ mkdir build
$ cd build
$ cmake .. -G Xcode -DCMAKE_TOOLCHAIN_FILE=../../ios.toolchain.cmake -DPLATFORM=OS
$ cmake --build . --config Release

# 如何判断静态库是否支持64位
$ lipo -info ./Debug-iphoneos/libspdlogd.a
Non-fat file: ./Debug-iphoneos/libspdlogd.a is architecture: arm64
