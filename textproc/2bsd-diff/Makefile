PORTNAME=	diff
PORTVERSION=	2.11.1
PORTREVISION=	2
CATEGORIES=	textproc
MASTER_SITES=	https://www.tuhs.org/Archive/Distributions/UCB/2.11BSD/ \
		http://www.d20hobbies.com/2.11BSD/
PKGNAMEPREFIX=	2bsd-
DISTNAME=	file8

MAINTAINER=	risner@stdio.com
COMMENT=	2.11BSD diff utility

CFLAGS+=	-fcommon -Wno-error=return-type
EXTRACT_AFTER_ARGS=	bin/diff man/man1/diff.1
WRKSRC=		${WRKDIR}/bin/diff

PLIST_FILES=	bin/2diff \
		libexec/2diffh \
		share/man/man1/2diff.1.gz

post-patch:
	@${REINPLACE_CMD} -e 's,%%PREFIX%%,${PREFIX},g' \
				${WRKSRC}/../../man/man1/diff.1

.include <bsd.port.mk>
