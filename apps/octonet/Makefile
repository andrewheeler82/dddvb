all: ddtest octonet octokey ddflash ddupdate

install: all
	install -m 0755 ddtest $(DESTDIR)/usr/bin
	install -m 0755 octonet $(DESTDIR)/usr/bin
	install -m 0755 octokey $(DESTDIR)/usr/bin
	install -m 0755 ddflash $(DESTDIR)/usr/bin
	install -m 0755 ddupdate $(DESTDIR)/usr/bin

ddflash: ddflash.c flash.h flash.c
	$(CC) -o ddflash ddflash.c

ddtest: ddtest.c flash.h flash.c
	$(CC) -o ddtest ddtest.c

ddupdate: ddupdate.c flash.h flash.c
	$(CC) -o ddupdate ddupdate.c

octonet: octonet.c
	$(CC) -o octonet octonet.c

octokey: octokey.c
	$(CC) -o octokey octokey.c

