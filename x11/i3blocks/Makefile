# Created by: Minbari <coszminv@gmail.com>
# $FreeBSD$

PORTNAME=	i3blocks
DISTVERSION=	1.5
CATEGORIES=	x11

MAINTAINER=	coszminv@gmail.com
COMMENT=	Define blocks for your i3bar status line

LICENSE=	GPLv3

USES=          gmake localbase tar:bzip2

USE_GITHUB=	yes
GH_ACCOUNT=	Minbar1
GH_TAGNAME=	fcee4e0

do-install:
	${INSTALL_PROGRAM} ${WRKSRC}/i3blocks ${STAGEDIR}${PREFIX}/bin/i3blocks
	${INSTALL_DATA} ${WRKSRC}/i3blocks.conf \
			${STAGEDIR}${PREFIX}/etc/i3blocks.conf.sample

post-install:
	${MKDIR} ${STAGEDIR}${DOCSDIR}
	${INSTALL_MAN} ${WRKSRC}/i3blocks.1.md ${STAGEDIR}${DOCSDIR}

.include <bsd.port.mk>
