# $FreeBSD$

PORTNAME=	react-rails
PORTVERSION=	2.2.1
CATEGORIES=	devel rubygems
MASTER_SITES=	RG
PKGNAMESUFFIX=	-rails5

MAINTAINER=	ruby@FreeBSD.org
COMMENT=	React/JSX adapter for the Ruby on Rails asset pipeline

LICENSE=	APACHE20
LICENSE_FILE=	${WRKSRC}/LICENSE

RUN_DEPENDS=	rubygem-babel-transpiler>=0.7.0:textproc/rubygem-babel-transpiler \
		rubygem-connection_pool>=0:net/rubygem-connection_pool \
		rubygem-execjs>=0:devel/rubygem-execjs \
		rubygem-railties5>0:www/rubygem-railties5 \
		rubygem-tilt>=0:devel/rubygem-tilt

NO_ARCH=	yes

USE_RUBY=	yes
USES=		gem

.include <bsd.port.mk>
