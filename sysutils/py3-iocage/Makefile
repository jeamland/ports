# Created by: Brandon Loves Sauce <brandon@ixsystems.com>
# $FreeBSD$

PORTNAME=	iocage
PORTVERSION=	${PRODUCT_VERSION:C/\-.*//:C/\_.*//}
PORTREVISION=	${REVISION}
CATEGORIES=	sysutils python
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}
EXTRACT_ONLY=

MAINTAINER=	brandon@ixsystems.com
COMMENT=	FreeBSD jail manager written in Python

LICENSE=	BSD2CLAUSE
LICENSE_FILE=	${WRKSRC}/LICENSE

BUILD_DEPENDS=	${PYTHON_PKGNAMEPREFIX}pytest-runner>=2.0.0:devel/py-pytest-runner
RUN_DEPENDS=	${PYTHON_PKGNAMEPREFIX}click>=6.7:devel/py-click \
	${PYTHON_PKGNAMEPREFIX}tqdm>=4.10.0:misc/py-tqdm \
	${PYTHON_PKGNAMEPREFIX}coloredlogs>0:devel/py-coloredlogs \
	ca_root_nss>0:security/ca_root_nss \
	${PYTHON_PKGNAMEPREFIX}texttable>=0.8.7:textproc/py-texttable \
	${PYTHON_PKGNAMEPREFIX}pytest-runner>=2.0.0:devel/py-pytest-runner \
	${PYTHON_PKGNAMEPREFIX}requests>=2.11.1:www/py-requests \
	${PYTHON_PKGNAMEPREFIX}libzfs>=1.0:devel/py-libzfs \
	${PYTHON_PKGNAMEPREFIX}dulwich>=0.18.6:devel/dulwich \
	${PYTHON_PKGNAMEPREFIX}netifaces>=0.10.6:net/py-netifaces
	

CONFLICTS=  py-iocage-[0-9]* iocage-[0-9]* iocage-devel-[0-9]*

NO_CHECKSUM=yes
WRKSRC=/usr/iocage_src

NO_ARCH=	yes
USES=		python
USE_PYTHON=	autoplist distutils

checksum fetch:
	${ECHO_CMD} ${.TARGET} not needed because building direct

.include <bsd.port.mk>
