```
$ tree --gitignore .
.
├── meson.build
├── README.md
└── src
    ├── msp430
    │   └── reset_reason.cpp
    └── msp430_reset_reason.cpp

2 directories, 4 files
```

```console
$ ~/tools/meson/meson.py setup --reconfigure buildDir
The Meson build system
Version: 1.7.99
Source dir: /home/user/meson_path_naming_bug
Build dir: /home/user/meson_path_naming_bug/buildDir
Build type: native build
Project name: meson_path_naming_bug
Project version: undefined
C++ compiler for the host machine: ccache c++ (gcc 11.4.0 "c++ (Ubuntu 11.4.0-1ubuntu1~22.04) 11.4.0")
C++ linker for the host machine: c++ ld.bfd 2.38
Host machine cpu family: x86_64
Host machine cpu: x86_64
Build targets in project: 1

Found ninja-1.10.1 at /usr/bin/ninja

ERROR: Multiple producers for Ninja target "exe.p/src_msp430_reset_reason.cpp.o". Please rename your targets.

A full log can be found at /home/user/meson_path_naming_bug/buildDir/meson-logs/meson-log.txt
```
