# This Makefile.am is in the public domain

SUBDIRS = include incl_priv mhd2 tests .

if RUN_LIBCURL_TESTS
#SUBDIRS += testcurl
if RUN_ZZUF_TESTS
#SUBDIRS += testzzuf
endif
endif

# Finally (last!) also build experimental lib...
if HAVE_EXPERIMENTAL
SUBDIRS += microhttpd_ws
endif

if BUILD_EXAMPLES
SUBDIRS += examples
endif

if BUILD_TOOLS
#SUBDIRS += tools
endif

EXTRA_DIST = \
 datadir/cert-and-key.pem \
 datadir/cert-and-key-for-wireshark.pem

.NOTPARALLEL:
