PORTNAME=	iohexperimenter
PORTVERSION=	0.2.9.2
PORTREVISION=	3
CATEGORIES=	math python
MASTER_SITES=	PYPI
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}
DISTNAME=	IOHexperimenter-${PORTVERSION}

MAINTAINER=	sunpoet@FreeBSD.org
COMMENT=	Experimenter for Iterative Optimization Heuristic
WWW=		https://github.com/IOHprofiler/IOHexperimenter

LICENSE=	GPLv3
LICENSE_FILE=	${WRKSRC}/LICENSE.txt

BUILD_DEPENDS=	${PYTHON_PKGNAMEPREFIX}setuptools>=0:devel/py-setuptools@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}wheel>=0:devel/py-wheel@${PY_FLAVOR}
RUN_DEPENDS=	${PYTHON_PKGNAMEPREFIX}numpy>=0,1:math/py-numpy@${PY_FLAVOR}

USES=		compiler:c++14-lang dos2unix python
USE_PYTHON=	autoplist concurrent pep517 unittest

USE_CXXSTD=	c++14
TEST_ENV=	PYTHONPATH=${STAGEDIR}${PYTHON_SITELIBDIR}/IOHexperimenter

post-install:
	${FIND} ${STAGEDIR}${PYTHON_SITELIBDIR} -name '*.so' -exec ${STRIP_CMD} {} +

.include <bsd.port.mk>
