# llvm-windows-full-builds
LLVM for Windows, which include the tools left out in the original releases.

Because of the resources involved with a full LLVM build, this repository saves you the effort and resources by providing **full bundles of the Windows (x86-64) build of core LLVM**. Note that other LLVM project tools and applications (such as Clang, lld, etc) are excluded. These builds are mainly intended for use in building other applications or libraries that link to LLVM.

This repository holds only this very README with the download options for each build; sources of the respective builds are provided as URLs to the LLVM repository.

## Contents
Each version has two distinct build types, each varying in size and usefulness. If you don't know which to pick, grab `RelWithDebInfo` if you're using LLVM's API, and use `Release` if you just want the missing binaries (such as `llvm-as.exe`, `llvm-dis.exe` and friends).

Each archive contains the following:
 - `/bin`, which holds the binaries (such as `llvm-dis.exe`);
 - `/include`, which holds the include headers for that particular LLVM version;
 - and `/lib`, which contains the static libraries that you can link against.
 
## Installation
These distributions are simple `.zip` files, so all you have to do is put the files somewhere and either add the path to `/bin` to your `PATH`-environment var, or provide the direct path to whatever tool/pipeline you're working with.

An example path is `C:\Program Files\LLVM`, which is where the Windows installer puts them by default and is most likely to be picked up by automatic discovery in tools or compilers.

## Hotlinking Warning :warning:
**None of the URLs are guaranteed to be valid forever**, and you're not advised to use them in automated installers. If you wish to include the binaries as part of your pipeline or the likes, reupload the contents elsewhere to be under your control.

## LLVM Windows Releases
Please do not file an issue when the "latest" version isn't the latest; these binaries are provided on an as-is basis and get updated on our own schedule.
### 15.0.3 (latest, Oct 18, 2022)
| File | Size | SHA256 |
|-|-|-|
|[15.0.3-Release.zip](https://s3.eu-central-1.wasabisys.com/bitgate-public/15.0.3-Release.zip)|865.31 MB|N/A|
|[15.0.3-RelWithDebInfo.zip](https://s3.eu-central-1.wasabisys.com/bitgate-public/15.0.3-RelWithDebInfo.zip)|1.64 GB|N/A|

### 14.0.6 (Jun 25, 2022)
| File | Size | SHA256 |
|-|-|-|
|[14.0.6-Release.zip](https://s3.eu-central-1.wasabisys.com/bitgate-public/14.0.6-Release.zip)|796.09 MB|N/A|
|[14.0.6-RelWithDebInfo.zip](https://s3.eu-central-1.wasabisys.com/bitgate-public/14.0.6-RelWithDebInfo.zip)|1.57 GB|N/A|
