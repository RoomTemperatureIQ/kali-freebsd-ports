# Created by: Vaida Bogdan
# $FreeBSD: head/security/dmitry/Makefile 386312 2015-05-14 10:15:04Z mat $

PORTNAME=	dmitry
PORTVERSION=	1.3a
CATEGORIES=	security
MASTER_SITES=	PACKETSTORM/UNIX/misc
DISTNAME=	DMitry-${PORTVERSION}

MAINTAINER=	ports@FreeBSD.org
COMMENT=	Deepmagic Information Gathering Tool

GNU_CONFIGURE=	yes
CONFIGURE_ARGS=	--prefix=${PREFIX}

PLIST_FILES=	bin/dmitry man/man1/dmitry.1.gz
PORTDOCS=	AUTHORS COPYING ChangeLog INSTALL NEWS README

OPTIONS_DEFINE=	DOCS

post-install:
	@${MKDIR} ${STAGEDIR}${DOCSDIR}
	${INSTALL_DATA} ${PORTDOCS:S|^|${WRKSRC}/|} ${STAGEDIR}${DOCSDIR}

.include <bsd.port.mk>
