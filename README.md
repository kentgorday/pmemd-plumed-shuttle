# pmemd-plumed-shuttle
Two small *barely tested* patches to Amber's pmemd.cuda and PLUMED to copy only relevant coordinates off the GPU for a small speedup.

Requires the shuttle transfer functions added in Amber 20, and this has been mostly tested with Amber 20 patch 12 + PLUMED 2.7.2 around October 2021. Only a small number of PLUMED actions have been tested.

This may have been inspired by [this mailing list message](http://archive.ambermd.org/202101/0207.html), I can't remember.

amber20\_src.patch patches the single file src/pmemd/src/runmd.F90

src.patch patches several files in PLUMED's src/core

Please test before using at your own risk.
