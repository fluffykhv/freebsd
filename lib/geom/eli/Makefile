# $FreeBSD$

PACKAGE=runtime
.PATH: ${.CURDIR:H:H}/misc ${SRCTOP}/sys/geom/eli ${SRCTOP}/sys/crypto/sha2

GEOM_CLASS=	eli
SRCS=	g_eli_crypto.c
SRCS+=	g_eli_hmac.c
SRCS+=	g_eli_key.c
SRCS+=	pkcs5v2.c
SRCS+=	sha256c.c
SRCS+=	sha512c.c

LIBADD=	md crypto

CFLAGS+=-I${SRCTOP}/sys
CFLAGS+=-I${SRCTOP}/crypto/openssl/include
CFLAGS+=-I${.OBJDIR:H:H:H}/secure/lib/libcrypto

.include <bsd.lib.mk>
