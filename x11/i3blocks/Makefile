# Created by: Minbari <coszminv@gmail.com>
# $FreeBSD$

PORTNAME=	i3blocks
DISTVERSION=	1.5
CATEGORIES=	x11

MAINTAINER=	coszminv@gmail.com
COMMENT=	Define blocks for your i3bar status line

LICENSE=	GPLv3

CFLAGS +=	-I${LOCALBASE}/include
USES=		gmake tar:bzip2

USE_GITHUB=	yes
GH_ACCOUNT=	Minbar1
GH_PROJECT=	i3blocks
GH_TAGNAME=	 3ad5d00

PLIST_FILES=	bin/i3blocks

do-install:
	${INSTALL_PROGRAM} ${WRKSRC}/i3blocks ${STAGEDIR}${PREFIX}/bin/i3blocks

.include <bsd.port.mk>
