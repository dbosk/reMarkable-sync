.PHONY: all
all: rM.pdf

rM.pdf: rM.tex rM.bib
rM.pdf: abstract.tex

rM.tex: rM.nw


.PHONY:
all: rM

rM.py: rM.nw
rM: rM.py
	cp $^ $@
	chmod +x $@


.PHONY: clean
clean:
	${RM} rM rM.py rM.pdf rM.tex


PKG_NAME-main= 			rM
PKG_FILES-main= 		rM
PKG_PREFIX-main= 		/usr/local
PKG_DIR-main= 			/bin
PKG_TARBALL_FILES-main= ${PKG_FILES-main} Makefile


INCLUDE_MAKEFILES=../makefiles
include ${INCLUDE_MAKEFILES}/tex.mk
include ${INCLUDE_MAKEFILES}/noweb.mk
include ${INCLUDE_MAKEFILES}/pkg.mk
