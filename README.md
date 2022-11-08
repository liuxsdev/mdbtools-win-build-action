# mdbtools-win-build-action

MDBTools built for Windows using MSYS2 and Github Action

Read the [mdbtools](https://github.com/mdbtools/mdbtools) guide about [build from source](https://github.com/mdbtools/mdbtools/blob/dev/README.md#from-source)

And windows build guide: [lsgunth/mdbtools-win](https://github.com/lsgunth/mdbtools-win)

## Build Info

| Name                      | Discription                                                                                           | Build Artifacts                                                                                                                                                                                                                              |
| ------------------------- | ----------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| build_mingw32.yml         | MINGW32 Build                                                                                         | [![Build MINGW32](https://github.com/liuxsdev/mdbtools-win-build-action/actions/workflows/build_mingw32.yml/badge.svg)](https://github.com/liuxsdev/mdbtools-win-build-action/actions/workflows/build_mingw32.yml)                           |
| build_mingw64.yml         | MINGW64 Build                                                                                         | [![Build MINGW64](https://github.com/liuxsdev/mdbtools-win-build-action/actions/workflows/build_mingw64.yml/badge.svg)](https://github.com/liuxsdev/mdbtools-win-build-action/actions/workflows/build_mingw64.yml)                           |
| build_mingw32_replace.yml | replace `…`(U+2026) [Horizontal Ellipsis](https://unicode-table.com/cn/2026/) character MINGW32 Build | [![Build MINGW32 (Replace)](https://github.com/liuxsdev/mdbtools-win-build-action/actions/workflows/build_mingw32_replace.yml/badge.svg)](https://github.com/liuxsdev/mdbtools-win-build-action/actions/workflows/build_mingw32_replace.yml) |
| build_mingw64_replace.yml | replace `…`(U+2026) [Horizontal Ellipsis](https://unicode-table.com/cn/2026/) character MINGW64 Build | [![Build MINGW64 (tweak)](https://github.com/liuxsdev/mdbtools-win-build-action/actions/workflows/build_mingw64_tweak.yml/badge.svg)](https://github.com/liuxsdev/mdbtools-win-build-action/actions/workflows/build_mingw64_tweak.yml)       |

## Other

When GCC was upgraded to version 12, build errors started appearing, so I tried downgrading from GCC 12 to 11.3.

Refer to this issue: [Cannot downgrade from GCC 12 to 11.3 #11730](https://github.com/msys2/MINGW-packages/issues/11730)

This website [https://repo.msys2.org/mingw/](https://repo.msys2.org/mingw/) contains old version packages

## Test

git clone https://github.com/mdbtools/mdbtestdata.git test
