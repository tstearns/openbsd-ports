# $OpenBSD$

COMMENT =	create ASCII graphical histograms in the terminal

GH_ACCOUNT =	philovivero
GH_PROJECT =	distribution
GH_TAGNAME =	v1.2.2

CATEGORIES =	textproc

NO_BUILD =	True

# tests don't work, see https://github.com/philovivero/distribution/issues/10
NO_TEST =	True

# GPLv2
PERMIT_PACKAGE_CDROM =	Yes

do-install:
	${INSTALL_SCRIPT} ${WRKSRC}/distribution ${PREFIX}/bin
	${INSTALL_DATA_DIR} ${PREFIX}/share/doc/distribution
	${INSTALL_DATA} ${WRKSRC}/LICENSE.md ${PREFIX}/share/doc/distribution
	${INSTALL_DATA} ${WRKSRC}/README.md ${PREFIX}/share/doc/distribution

.include <bsd.port.mk>
