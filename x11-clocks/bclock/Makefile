PORTNAME=	bclock
PORTVERSION=	1.0
PORTREVISION=	3
CATEGORIES=	x11-clocks
MASTER_SITES=	SUNSITE/X11/clocks

MAINTAINER=	ports@FreeBSD.org
COMMENT=	Round, analog X11 clock with Bezier curve hands

USES=		imake xorg
USE_XORG=	ice sm x11 xext xmu xt

PLIST_FILES=	bin/bclock \
		lib/X11/app-defaults/Clock-color \
		share/man/man1/${PORTNAME}.1.gz

.include <bsd.port.mk>
