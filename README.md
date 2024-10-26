# maptools_patched_debian
Contributors: Jamey Harris coldicefisher@gmail.com

R maptools patched and tested on Ubuntu 22. This is a patched version of R maptools as of 
2024-10-26.

## Bug Fix error(msg):

src/Rgshhs.c: Lines 101, 341
error(msg);

Updated to:
error("Error: %s", msg);


## Install

```bash
git clone git@github.com:coldicefisher/maptools_patched_debian.git

cd maptools_patched_debian

sudo R
```

Onse inside the R CLI, run:

```r
install.packages("maptools_1.1-8.tar.gz", repos=NULL, type="source")
```

## Compile from source

If you need to make changes to the source code, you can compile and  make a tarball:

```bash
sudo R CMD build .
```
## Instructions to install ggsn

To be written...
