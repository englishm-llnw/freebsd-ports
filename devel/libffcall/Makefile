# Created by: jagapen@home.com
# $FreeBSD$

PORTNAME=	libffcall
PORTVERSION=	1.13
CATEGORIES=	devel
MASTER_SITES=	GNU/${PORTNAME}

MAINTAINER=	amutu@amutu.com
COMMENT=	Foreign function call libraries

LICENSE=	GPLv2+

GNU_CONFIGURE=	yes
USES=		gmake libtool
USE_LDCONFIG=	yes

CONFIGURE_ARGS=	--enable-shared
CONFIGURE_TARGET=	${ARCH:S/amd64/x86_64/}-portbld-${OPSYS:tl}${OSREL}
MAKE_JOBS_UNSAFE=	yes

CFLAGS+=	-fPIC

post-install:
	@${STRIP_CMD} ${STAGEDIR}${PREFIX}/lib/libavcall.so \
		${STAGEDIR}${PREFIX}/lib/libcallback.so \
		${STAGEDIR}${PREFIX}/lib/libtrampoline.so

.include <bsd.port.mk>
