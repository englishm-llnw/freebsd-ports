# Created by: Eugene Grosbein <ports@grosbein.net>
# $FreeBSD$

PORTNAME=	msrplib
PORTVERSION=	0.14.4
PORTREVISION=	1
CATEGORIES=	net python
MASTER_SITES=	http://download.ag-projects.com/SipClient/ \
		http://www.grosbein.net/python/
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}
DISTNAME=	python-${PORTNAME}-${PORTVERSION}

MAINTAINER=	eugen@FreeBSD.org
COMMENT=	Python MSRP client library

LICENSE=	GPLv2
LICENSE_FILE=	${WRKSRC}/LICENSE

BUILD_DEPENDS=	${PYTHON_PKGNAMEPREFIX}gnutls>=1.1.6:security/py-gnutls \
		${PYTHON_PKGNAMEPREFIX}eventlet>=0.9.15:net/py-eventlet \
		${PYTHON_PKGNAMEPREFIX}application>=1.1.0:devel/py-application
RUN_DEPENDS:=	${BUILD_DEPENDS}

NO_ARCH=	yes
USES=		python twisted:names
USE_PYTHON=	distutils autoplist

.include <bsd.port.mk>
