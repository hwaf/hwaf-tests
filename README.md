hwaf-tests
==========

A simple multi-projects set of tests for ``hwaf``.

Instructions
-------------

```sh
$ ./doit

::: running test...
::::::::::::::::::::::
::: building proj-a...
~/dev/atlas/mana/git/hwaf-tests/proj-a ~/dev/atlas/mana/git/hwaf-tests
Setting top to                           : /home/binet/dev/atlas/mana/git/hwaf-tests/proj-a 
Setting out to                           : /home/binet/dev/atlas/mana/git/hwaf-tests/proj-a/__build__ 
Checking for 'gcc' (c compiler)          : /usr/bin/gcc 
Checking for 'g++' (c++ compiler)        : /usr/bin/g++ 
================================================================================
project                                  : proj-a 
prefix                                   : /opt/sw/mana/proj-a 
destdir                                  : /home/binet/dev/atlas/mana/git/hwaf-tests/install-area 
pkg dir                                  : pkg 
variant                                  : x86_64-linux-gcc-opt 
arch                                     : x86_64 
OS                                       : linux 
compiler                                 : gcc 
build-type                               : opt 
projects deps                            : None 
================================================================================
Checking for 'gcc' (c compiler)          : /usr/bin/gcc 
Checking for program python2             : /usr/bin/python2 
checking for __extern_always_inline      : ok 
Checking for program python              : /usr/bin/python2 
python executable '/usr/bin/python2' differs from system '/usr/bin/python'
Checking for python version              : (2, 7, 3, 'final', 0) 
Checking for library python2.7 in LIBDIR : yes 
Checking for program /usr/bin/python2-config,python2.7-config,python-config-2.7,python2.7m-config : /usr/bin/python2-config 
Checking for header Python.h             : yes 
Checking for header xrootd/XrdVersion.hh : not found 
Checking for program xml2-config         : /usr/bin/xml2-config 
Checking for 'xml2-config'               : yes 
Found xml2 at                            : (local environment) 
Checking xml2 version                    : ok 
libxml2 version                          : 2.8.0 
Checking for program root-config         : /usr/bin/root-config 
Checking for '/usr/bin/root-config'      : yes 
Found root at                            : (local environment) 
Checking for program genmap              : /usr/bin/genmap 
Checking for program genreflex           : /usr/bin/genreflex 
Checking for program root                : /usr/bin/root 
Checking for program rootcint            : /usr/bin/rootcint 
Checking for program gccxml              : /usr/bin/gccxml 
GCCXML version                           : 0.9.0 
Checking ROOT version                    : ok 
ROOT version                             : 5.34/03 
Checking for ROOT::TH1                   : yes 
Checking for ROOT::TTree                 : yes 
Checking for pyroot-cxx                  : yes 
Checking for reflex                      : yes 
Checking for cintex                      : yes 
Checking for $ROOTSYS                    : /usr 
Python module ROOT                       : ok 
Python module PyCintex                   : ok 
Checking for library m                   : yes 
Found m at                               : (local environment) 
Checking for library dl                  : yes 
Found dl at                              : (local environment) 
Checking for library pthread             : yes 
Found pthread at                         : (local environment) 
Checking for header zlib.h               : yes 
Found zlib at                            : (local environment) 
Checking for header bfd.h                : yes 
Found bfd at                             : (local environment) 
Checking for library rt                  : yes 
Found rt at                              : (local environment) 
Checking bfd_init                        : ok 
Checking for header tbb/tbb.h            : yes 
Found tbb at                             : (local environment) 
Checking tbb version                     : ok 
TBB version                              : 4.1 
Checking tbb linking                     : ok 
TBB runtime interface                    : 6101 
'configure' finished successfully (7.037s)
Waf: Entering directory `/home/binet/dev/atlas/mana/git/hwaf-tests/proj-a/__build__'
ROOT-home: /usr
[1/6] cxx: pkg/posixcomps/src/fpe.cxx -> __build__/pkg/posixcomps/src/fpe.cxx.1.o
[2/6] cxx: pkg/rootcomps/src/rootcomps.cxx -> __build__/pkg/rootcomps/src/rootcomps.cxx.1.o
[3/6] cxx: pkg/tbb/src/tbb-hello.cxx -> __build__/pkg/tbb/src/tbb-hello.cxx.1.o
[4/6] cxxshlib: __build__/pkg/posixcomps/src/fpe.cxx.1.o -> __build__/pkg/posixcomps/libbfd-fpe.so
[5/6] cxxshlib: __build__/pkg/rootcomps/src/rootcomps.cxx.1.o -> __build__/pkg/rootcomps/librootcomps.so
[6/6] cxxprogram: __build__/pkg/tbb/src/tbb-hello.cxx.1.o -> __build__/pkg/tbb/tbb-hello
Waf: Leaving directory `/home/binet/dev/atlas/mana/git/hwaf-tests/proj-a/__build__'
'build' finished successfully (0.644s)
Waf: Entering directory `/home/binet/dev/atlas/mana/git/hwaf-tests/proj-a/__build__'
ROOT-home: /usr
+ install /home/binet/dev/atlas/mana/git/hwaf-tests/install-area/opt/sw/mana/proj-a/include/rootcomps/test-h1d.hh (from pkg/rootcomps/inc/rootcomps/test-h1d.hh)
+ install /home/binet/dev/atlas/mana/git/hwaf-tests/install-area/opt/sw/mana/proj-a/lib/libbfd-fpe.so (from __build__/pkg/posixcomps/libbfd-fpe.so)
+ install /home/binet/dev/atlas/mana/git/hwaf-tests/install-area/opt/sw/mana/proj-a/project.info (from __build__/project.info)
+ install /home/binet/dev/atlas/mana/git/hwaf-tests/install-area/opt/sw/mana/proj-a/lib/librootcomps.so (from __build__/pkg/rootcomps/librootcomps.so)
+ install /home/binet/dev/atlas/mana/git/hwaf-tests/install-area/opt/sw/mana/proj-a/bin/tbb-hello (from __build__/pkg/tbb/tbb-hello)
Waf: Leaving directory `/home/binet/dev/atlas/mana/git/hwaf-tests/proj-a/__build__'
'install' finished successfully (0.028s)
Waf: Entering directory `/home/binet/dev/atlas/mana/git/hwaf-tests/proj-a/__build__'
ROOT-home: /usr
+ install /home/binet/dev/atlas/mana/git/hwaf-tests/proj-a/__build__/bdist_tmp_dir/opt/sw/mana/proj-a/include/rootcomps/test-h1d.hh (from pkg/rootcomps/inc/rootcomps/test-h1d.hh)
+ install /home/binet/dev/atlas/mana/git/hwaf-tests/proj-a/__build__/bdist_tmp_dir/opt/sw/mana/proj-a/project.info (from __build__/project.info)
+ install /home/binet/dev/atlas/mana/git/hwaf-tests/proj-a/__build__/bdist_tmp_dir/opt/sw/mana/proj-a/lib/librootcomps.so (from __build__/pkg/rootcomps/librootcomps.so)
+ install /home/binet/dev/atlas/mana/git/hwaf-tests/proj-a/__build__/bdist_tmp_dir/opt/sw/mana/proj-a/lib/libbfd-fpe.so (from __build__/pkg/posixcomps/libbfd-fpe.so)
+ install /home/binet/dev/atlas/mana/git/hwaf-tests/proj-a/__build__/bdist_tmp_dir/opt/sw/mana/proj-a/bin/tbb-hello (from __build__/pkg/tbb/tbb-hello)
Waf: Leaving directory `/home/binet/dev/atlas/mana/git/hwaf-tests/proj-a/__build__'
New archive created: proj-a-x86_64-linux-gcc-opt-0.0.1.tar.gz
'bdist' finished successfully (0.057s)
-rwxr-xr-x root/root     36086 2012-12-04 17:29 opt/sw/mana/proj-a/bin/tbb-hello
-rw-r--r-- root/root       114 2012-12-04 10:04 opt/sw/mana/proj-a/include/rootcomps/test-h1d.hh
-rwxr-xr-x root/root      6201 2012-12-04 17:29 opt/sw/mana/proj-a/lib/libbfd-fpe.so
-rwxr-xr-x root/root     10654 2012-12-04 17:29 opt/sw/mana/proj-a/lib/librootcomps.so
-rw-r--r-- root/root     11009 2012-12-04 17:29 opt/sw/mana/proj-a/project.info
~/dev/atlas/mana/git/hwaf-tests

::::::::::::::::::::::
::: building proj-b...
~/dev/atlas/mana/git/hwaf-tests/proj-b ~/dev/atlas/mana/git/hwaf-tests
Setting top to                           : /home/binet/dev/atlas/mana/git/hwaf-tests/proj-b 
Setting out to                           : /home/binet/dev/atlas/mana/git/hwaf-tests/proj-b/__build__ 
Checking for 'gcc' (c compiler)          : /usr/bin/gcc 
Checking for 'g++' (c++ compiler)        : /usr/bin/g++ 
could not locate project at [/not/there]
================================================================================
project                                  : proj-b 
prefix                                   : /opt/sw/mana/proj-b 
destdir                                  : /home/binet/dev/atlas/mana/git/hwaf-tests/install-area 
pkg dir                                  : pkg 
variant                                  : x86_64-linux-gcc-opt 
arch                                     : x86_64 
OS                                       : linux 
compiler                                 : gcc 
build-type                               : opt 
projects deps                            : proj-a 
================================================================================
'configure' finished successfully (0.128s)
Waf: Entering directory `/home/binet/dev/atlas/mana/git/hwaf-tests/proj-b/__build__'
ROOT-home: /usr
[1/2] cxx: pkg/rootcomps-b/src/th1d.cxx -> __build__/pkg/rootcomps-b/src/th1d.cxx.1.o
[2/2] cxxshlib: __build__/pkg/rootcomps-b/src/th1d.cxx.1.o -> __build__/pkg/rootcomps-b/libprojb-rootcomps.so
Waf: Leaving directory `/home/binet/dev/atlas/mana/git/hwaf-tests/proj-b/__build__'
'build' finished successfully (0.411s)
Waf: Entering directory `/home/binet/dev/atlas/mana/git/hwaf-tests/proj-b/__build__'
ROOT-home: /usr
+ install /home/binet/dev/atlas/mana/git/hwaf-tests/install-area/opt/sw/mana/proj-b/project.info (from __build__/project.info)
+ install /home/binet/dev/atlas/mana/git/hwaf-tests/install-area/opt/sw/mana/proj-b/lib/libprojb-rootcomps.so (from __build__/pkg/rootcomps-b/libprojb-rootcomps.so)
Waf: Leaving directory `/home/binet/dev/atlas/mana/git/hwaf-tests/proj-b/__build__'
'install' finished successfully (0.019s)
Waf: Entering directory `/home/binet/dev/atlas/mana/git/hwaf-tests/proj-b/__build__'
ROOT-home: /usr
+ install /home/binet/dev/atlas/mana/git/hwaf-tests/proj-b/__build__/bdist_tmp_dir/opt/sw/mana/proj-b/project.info (from __build__/project.info)
+ install /home/binet/dev/atlas/mana/git/hwaf-tests/proj-b/__build__/bdist_tmp_dir/opt/sw/mana/proj-b/lib/libprojb-rootcomps.so (from __build__/pkg/rootcomps-b/libprojb-rootcomps.so)
Waf: Leaving directory `/home/binet/dev/atlas/mana/git/hwaf-tests/proj-b/__build__'
New archive created: proj-b-x86_64-linux-gcc-opt-0.0.1.tar.gz
'bdist' finished successfully (0.028s)
-rwxr-xr-x root/root      8195 2012-12-04 17:29 opt/sw/mana/proj-b/lib/libprojb-rootcomps.so
-rw-r--r-- root/root     10331 2012-12-04 17:29 opt/sw/mana/proj-b/project.info
~/dev/atlas/mana/git/hwaf-tests

```
