# $OpenBSD$

COMMENT =	create ASCII graphical histograms in the terminal

GH_ACCOUNT =	philovivero
GH_PROJECT =	distribution
GH_TAGNAME =	1.3

CATEGORIES =	textproc

MAINTAINER =	Taylor Stearns <t@tstearns.com>

NO_BUILD =	True

# GPLv2
PERMIT_PACKAGE_CDROM =	Yes

do-install:
	${INSTALL_SCRIPT} ${WRKSRC}/distribution ${PREFIX}/bin
	${INSTALL_DATA_DIR} ${PREFIX}/share/doc/distribution
	${INSTALL_DATA} ${WRKSRC}/LICENSE.md ${PREFIX}/share/doc/distribution
	${INSTALL_DATA} ${WRKSRC}/README.md ${PREFIX}/share/doc/distribution

do-test:
	cd ${WRKSRC}/tests && distribution=${WRKSRC}/distribution ./runTests.sh

.include <bsd.port.mk>
