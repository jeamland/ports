# Created by: Antoine Brodin <antoine@FreeBSD.org>
# $FreeBSD$

PORTNAME=	pefile
PORTVERSION=	2017.8.1
CATEGORIES=	devel python
MASTER_SITES=	https://github.com/erocarrera/pefile/releases/download/v${PORTVERSION}/
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	antoine@FreeBSD.org
COMMENT=	Python module to read and work with PE files

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/LICENSE

BUILD_DEPENDS=	${PYTHON_PKGNAMEPREFIX}future>=0:devel/py-future
RUN_DEPENDS=	${PYTHON_PKGNAMEPREFIX}future>=0:devel/py-future

NO_ARCH=	yes
USES=		python
USE_PYTHON=	distutils autoplist

.include <bsd.port.mk>
