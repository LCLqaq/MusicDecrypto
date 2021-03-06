# MusicDecrypto

[![GitHub release](https://img.shields.io/github/release/davidxuang/musicdecrypto.svg)](https://GitHub.com/davidxuang/musicdecrypto/releases/)
[![Build status](https://ci.appveyor.com/api/projects/status/github/davidxuang/musicdecrypto?svg=true)](https://ci.appveyor.com/project/davidxuang/musicdecrypto)
[![GitHub license](https://img.shields.io/github/license/davidxuang/musicdecrypto.svg)](https://github.com/davidxuang/musicdecrypto/blob/master/LICENSE)

This project aims to implement music de-DRM for NetEase Cloud Music and QQ Music on .NET Core, and generate native executable through [CoreRT](https://github.com/dotnet/corert).

## Build

`dotnet build -c Release`

### Dependencies

-   [.NET Core](https://dotnet.microsoft.com) 3.1
-   [CommandLineParser](https://github.com/commandlineparser/commandline)
-   [Json.NET](https://www.newtonsoft.com/json)
-   [NLog](https://nlog-project.org/)
-   [TagLib#](https://github.com/mono/taglib-sharp)

## Run

Drag and drop files and/or directories into the executable or run:

`MusicDecrypto [options] path...`

### Options

- `-d, --skip-duplicate` Do not overwrite existing files.
- `-n, --force-rename` Try to fix Tencent file name basing on metadata.
- `-o, --output <directory>` Specify output directory.

## References

-   [ncmdump](https://github.com/anonymous5l/ncmdump)
-   [unlock-music](https://github.com/ix64/unlock-music)
