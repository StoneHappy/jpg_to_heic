# Jpeg To Heic


### How to build

install vcpkg

install libheif and libjpeg by vcpkg
```
vcpkg install libjpeg-turbo:x64-windows
vcpkg install libheif:x64-windows
```

```bash
git clone https://github.com/StoneHappy/jpg_to_heic.git

cd jpg_to_heic

mkdir build

cd build

cmake .. -DCMAKE_TOOLCHAIN_FILE=E:/softwares/vcpkg/scripts/buildsystems/vcpkg.cmake
 -DVCPKG_TARGET_TRIPLET=x64-windows

```

you must reassign follow path:

`-DCMAKE_TOOLCHAIN_FILE=E:/softwares/vcpkg/scripts/buildsystems/vcpkg.cmake`

``.sln`` file will generate in build directory. open it by Visual Studio and generate is.

### How to use

Executable file will be in jpg_to_heic/out/bin/

Type follow command to know usage;

```bash
.\jpgToHeic.exe -?
```