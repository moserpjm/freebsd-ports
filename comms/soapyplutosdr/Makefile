PORTNAME=	SoapyPlutoSDR
DISTVERSIONPREFIX=	soapy-plutosdr-
DISTVERSION=	0.2.2
CATEGORIES=	comms hamradio

MAINTAINER=	yuri@FreeBSD.org
COMMENT=	Soapy SDR plugin for PlutoSDR
WWW=		https://github.com/pothosware/SoapyPlutoSDR/wiki

LICENSE=	GPLv2
LICENSE_FILE=	${WRKSRC}/LICENSE

LIB_DEPENDS=	libiio.so:misc/libiio \
		libSoapySDR.so:misc/soapysdr

USES=		cmake compiler:c++11-lang pkgconfig
USE_GITHUB=	yes
GH_ACCOUNT=	pothosware

PLIST_FILES=	lib/SoapySDR/modules0.8/libPlutoSDRSupport.so

.include <bsd.port.mk>
