This directory contains the sources for each of the binary packages used by this
container.  These are the exact sources used to build the binaries in the
package.  To ensure you have the correct files, you can verify the checksums for
each with the `sha256sum` command:

```
09dad447b85ecb57debcb423f34381db7f112a010fbc83e4f65b3b31cf416514  alltray-0.7.5.1dev.tar.gz
8ceb4b9ee5adedde47b31e975c1d90c73ad27b6b165a1dcd80c7c545eb65b903  alltray-COPYING
231f7edcc7352d7734a96eef0b8030f77982678c516876fcb81e25b32d68564c  libgtop2-COPYING
851a993cfa559f262fa89a8f508d3267ce92a559ba86e8cb6530c963ae495c46  libgtop2_2.34.2-1.debian.tar.xz
66d641101ee80603e76afa1e39243c11a271f545bee417c28417b2de1691445e  libgtop2_2.34.2-1.dsc
268ad1478363e8c0955ea842fa134f6eb88965ab5e03166c20d8df9e7a1f8ef8  libgtop2_2.34.2.orig.tar.xz
2a63642709289dafa0573b48aaffb52d418c47df22312f384058031cb48b65bc  alltray
c730f2975dc7f596d10a25b0a0607e234546896a3d6af7934b8767dcc9784e36  libgtop-2.0.so.7.2.0
```

AllTray version 0.7.5.1 is the most recent version of AllTray I found that would
successfully dock with my current notification tray.  It carries a GPLv3
license, please see alltray-COPYING for details.

libgtop2 is a version that is compatibile with the build version of AllTray.
Later versions may or may not work for you.  It carries a GPLv2+ license,
meaning it may be distributed under the terms of the GPLv2 license or any later
version.  Please see libgtop2-COPYING for more details.
