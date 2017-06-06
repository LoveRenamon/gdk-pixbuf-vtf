gdk-pixbuf-vtf - Valve Texture Format PixBuf loader
===================================================

This fork makes it work with gtk3. For me at least.

Original created by Forrest Voight `<voights@gmail.com>`
Based on gdk-pixbuf-psd by Jan Dudek `<jd@jandudek.com>`.

## Build Instructions

```console
$ mkdir build
$ cd build
$ cmake ..
$ make
```

## Install Instructions

```console
$ sudo cp libpixbufloader-vtf.so /usr/lib/gdk-pixbuf-2.0/2.10.0/loaders/
$ sudo gdk-pixbuf-query-loaders --update-cache
$ cp x-vtf.xml ~/.local/share/mime/packages/
$ update-mime-database ~/.local/share/mime/
```

alternatively, there is a [PKGBUILD](https://gist.github.com/Rahix/72f13d5d7f534e35a3006a846651221d) for ArchLinux.
