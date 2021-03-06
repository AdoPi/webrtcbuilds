# webrtcbuilds
==============

The goal of webrtcbuilds is to provide a single standalone static library and
package for WebRTC.

## Current Platforms and Prerequisites

* OSX (highly recommend [Homebrew](http://brew.sh/) is installed)
* Windows (highly recommend [Visual Studio Community 2013]
(http://www.chromium.org/developers/how-tos/build-instructions-windows) at least
and a [Bash shell such as Git for Windows](https://msysgit.github.io) is
installed)
* Linux (tested on Ubuntu 16.04 64-bit)

## How to run

`./build.sh` to build the latest version of WebRTC.

Or with options.

```
Usage:
   ./build.sh [OPTIONS]

OPTIONS:
   -h             Show this message
   -d             Debug mode. Print all executed commands.
   -o OUTDIR      Output directory. Default is 'out'
   -b BRANCH      Latest revision on git branch. Overrides -r. Common branch names are 'branch-heads/nn', where 'n' is the release number.
   -r REVISION    Git SHA revision. Default is latest revision.
   -t TARGET OS   The target os for cross-compilation. Default is the host OS such as 'linux', 'mac', 'win'. Other values can be 'android', 'ios'.
   -c TARGET CPU  The target cpu for cross-compilation. Default is 'x64'. Other values can be 'x86', 'arm64', 'arm'.
```

## Where is the package

`out/webrtcbuilds-<rev>-<sha>-<target-os>-<target-cpu>.zip`
where `<rev>` is the revision number of the commit, `<sha>` is the short git SHA
of the commit, and `<target-os>-<target-cpu>` is the OS (linux, mac, win) and
CPU (x64, x86) of the target environment.

## Documentation

Wiki: https://github.com/vsimon/webrtcbuilds/wiki

Mailing List: http://groups.google.com/group/webrtcbuilds
