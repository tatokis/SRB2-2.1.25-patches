This repo contains patches needed to build the [last version of SRB2 2.1 (2.1.25)](https://github.com/STJr/SRB2/releases/tag/SRB2_release_2.1.25) with a modern compiler on Linux.

* srb2_gcc_11.patch
    * Fixes the following:
        ```
        /usr/bin/ld: CMakeFiles/SRB2SDL2.dir/__/b_bot.c.o:(.bss+0x0): multiple definition of `savegamename'; CMakeFiles/SRB2SDL2.dir/__/am_map.c.o:(.bss+0x0): first defined here
        /usr/bin/ld: CMakeFiles/SRB2SDL2.dir/__/b_bot.c.o:(.bss+0x100): multiple definition of `ntemprecords'; CMakeFiles/SRB2SDL2.dir/__/am_map.c.o:(.bss+0x100): first defined here
        /usr/bin/ld: CMakeFiles/SRB2SDL2.dir/__/d_clisrv.c.o:(.bss+0x100): multiple definition of `compat_special_music_slots'; CMakeFiles/SRB2SDL2.dir/__/console.c.o:(.bss+0x160): first defined here
        /usr/bin/ld: CMakeFiles/SRB2SDL2.dir/__/d_main.c.o:(.bss+0x1e0): multiple definition of `ms_RoomId'; CMakeFiles/SRB2SDL2.dir/__/d_clisrv.c.o:(.bss+0x1d8): first defined here
        [...]
        ```
