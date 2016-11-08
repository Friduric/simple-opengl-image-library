# About
Pre-built and working Simple OpenGL Image Library (SOIL) compatible with C++11. Compatible with Visual Studio 2015.

# How to use
**Add the "libs" and "include" folders to your project.** 

In Visual Studio (2010-2015) you also need to do the following:

1. `Project -> Properties -> VC++ Directories` -> **Add** `include` **to "Include Directories".**

2. `Project -> Properties -> VC++ Directories` -> **Add** `libs` **to "Library Directories".**

Alternatively:

1. `Project -> Properties -> C/C++` -> **Add** `include` **to "Additional Include Directories".**

2. `Project -> Properties -> Linker` -> **Add** `libs` **to "Additional Library Directories".**


Include SOIL (`#include <SOIL\SOIL.h>`) whenever you need to use SOIL.

# Other
This SOIL library correctly removes and solves the following (official SOIL lib) errors:

`1>LINK : warning LNK4098: defaultlib 'MSVCRT' conflicts with use of other libs; use /NODEFAULTLIB:library`

`1>libSOIL.lib(stb_image_aug.o) : error LNK2019: unresolved external symbol __alloca referenced in function
_stbi_zlib_decode_noheader_buffer`

`1>libSOIL.lib(image_helper.o) : error LNK2019: unresolved external symbol _sqrtf referenced in function _RGBE_to_RGBdivA2`

`1>SOIL.lib(stb_image_aug.o) : error LNK2019: unresolved external symbol __alloca referenced in function _stbi_zlib_decode_noheader_buffer`

`1>SOIL.lib(image_helper.o) : error LNK2019: unresolved external symbol _sqrtf referenced in function _RGBE_to_RGBdivA2`
