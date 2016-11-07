# About
Pre-built and working Simple OpenGL Image Library (SOIL) for modern C++11. Compatible with modern versions of Visual Studio.

# How to use
Simply add the "libs" and "include" folder to your project. 

In Visual Studio (2010-2015) you also need to do the following:
1. Project -> Properties -> VC++ Directories :: Add "includes" to "Include Directories".
2. Project -> Properties -> VC++ Directories :: Add "libs" to "Library Directories".
3. Project -> Properties -> C/C++ :: Add "includes\SOIL" to "Additional Include Directories".
4. Project -> Properties -> Linker :: Add "libs" to "Additional Library Directories".

Now simply write "#include <SOIL\SOIL.h>" whenever you need to use SOIL.

This should correctly remove the following errors with the official SOIL version:
1>LINK : warning LNK4098: defaultlib 'MSVCRT' conflicts with use of other libs; use /NODEFAULTLIB:library
1>libSOIL.lib(stb_image_aug.o) : error LNK2019: unresolved external symbol __alloca referenced in function _stbi_zlib_decode_noheader_buffer
1>libSOIL.lib(image_helper.o) : error LNK2019: unresolved external symbol _sqrtf referenced in function _RGBE_to_RGBdivA2
1>SOIL.lib(stb_image_aug.o) : error LNK2019: unresolved external symbol __alloca referenced in function _stbi_zlib_decode_noheader_buffer
1>SOIL.lib(image_helper.o) : error LNK2019: unresolved external symbol _sqrtf referenced in function _RGBE_to_RGBdivA2
