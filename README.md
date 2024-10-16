# PTPlayLibrary
Play ("decode") protracker modules

The reason for this repo's existance is that IMP3 (https://aminet.net/package/mus/play/imp3) can be made to use of tthe retargetable audio (AHI) to play modules.
The problem was that the ptplay.library as found on the Aminet would often crash when used in conjunction with PTReplayLibrary_AHI (the wrapper around PTPlayLibrary, not the PTReplayLibrary 6.6 or 7.0 which use Paula audio).
I've noticed that there was a slightly updated version for OS4, but there was no backport for OS3, so...

It was taken from https://aminet.net/package/mus/play/PTPlayLibrary.lha, diffed against https://aminet.net/util/libs/ptplaylib_os4.lha
and updated with some changes. The Makefile was adjusted to play nice with environmental variables and all that is in the git history.

I've built it on x86_64 with https://github.com/nicolasbauw/amiga-cc by clonning it to /opt and following the directions.





The original PTPlayLibrary.readme, as can be found on the Aminet.net:

Short:        Play ("decode") protracker modules
Author:       Ronald Hof, Timm S. Mueller, Per Johansson, Ilkka Lehtoranta (ilkleht@isoveli.org)
Uploader:     Ilkka Lehtoranta (ilkleht@isoveli.org)
Type:         mus/play
Version:      2.6
Architecture: m68k-amigaos; ppc-morphos

Changes in 2.6:
 - fixed division by zero exception on 680x0 CPUs (reported by Thilo K�hler)


ptplay.library is a library to play protracker modules. It is based on
work of Ronald Hof, Timm Mueller and Per Johansson with my own additions:

  - shared library
  - support for SoundTracker modules

However SoundTracker support is unfinished but since there are better
MOD player libraries for MorphOS I havent got motivation to finish it.
I also started working on SoundFX player but since Mahendra Tallur
created geronto.library my work is done ;)

This source code has been rotting on my HD about two years now so I think
it is about time to release it. AmigaOS users might find it interesting still.



