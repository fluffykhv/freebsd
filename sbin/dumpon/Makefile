# $FreeBSD$

.include <src.opts.mk>

PACKAGE=runtime
PROG=	dumpon

.if ${MK_OPENSSL} != "no"
LIBADD=	crypto
CFLAGS+= -DHAVE_CRYPTO
CFLAGS+= -I${SRCTOP}/crypto/openssl/include
CFLAGS+= -I${.OBJDIR:H:H}/secure/lib/libcrypto
.endif

MAN=	dumpon.8

.include <bsd.prog.mk>
