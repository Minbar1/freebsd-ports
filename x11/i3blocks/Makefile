# Created by: Minbari <coszminv@gmail.com>
# $FreeBSD$

PORTNAME=	i3blocks
DISTVERSION=	1.5
CATEGORIES=	x11

MAINTAINER=	coszminv@gmail.com
COMMENT=	Define blocks for your i3bar status line

LICENSE=	GPLv3

USES=		gmake
USE_GITHUB=	yes
GH_ACCOUNT=	Minbar1
GH_TAGNAME=	fcee4e0

post-install:
	${INSTALL_MAN} ${WRKSRC}/i3blocks.1.md ${STAGEDIR}${MANDIRS}/man1
	${MV} ${STAGEDIR}${PREFIX}/etc/i3blocks.conf \
		${STAGEDIR}${PREFIX}/etc/i3blocks.conf.sample

.include <bsd.port.mk>
