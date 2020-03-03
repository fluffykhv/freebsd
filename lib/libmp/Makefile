# $FreeBSD$

.include <src.opts.mk>

LIB=		mp
SHLIB_MAJOR=	7
LIBADD=		crypto
MAN=		libmp.3
INCS=		mp.h
SRCS=		mpasbn.c

CFLAGS+=	-I${SRCTOP}/crypto
CFLAGS+=	-I${SRCTOP}/crypto/openssl/include
CFLAGS+=	-I${.OBJDIR:H:H}/secure/lib/libcrypto

VERSION_DEF=	${SRCTOP}/lib/libc/Versions.def
SYMBOL_MAPS=	${.CURDIR}/Symbol.map

HAS_TESTS=
SUBDIR.${MK_TESTS}+= tests

.include <bsd.lib.mk>
