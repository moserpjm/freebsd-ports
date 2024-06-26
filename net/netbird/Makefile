PORTNAME=	netbird
PORTVERSION=	0.28.3
DISTVERSIONPREFIX=	v
CATEGORIES=	security net-vpn

WRKSRC=		${WRKDIR}/netbird-${PORTVERSION}

MAINTAINER=	moser@pjm.co.at
COMMENT=	Mesh VPN
WWW=		https://netbird.io/

USES=		go:1.22,modules

GOAMD64=v4

GO_MODULE=	github.com/netbirdio/netbird

USE_RC_SUBR=	netbird

GO_TARGET=	./client:netbird
GO_BUILDFLAGS=	-tags freebsd -o ${PORTNAME} -ldflags "\
		 -s -w -X github.com/netbirdio/netbird/version.version=${PORTVERSION}"

PLIST_FILES=	bin/netbird


.include <bsd.port.mk>
