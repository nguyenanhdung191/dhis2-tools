man: manual.xml
	mkdir -p ../pkg/usr/share/man/man1
	xsltproc /usr/share/xml/docbook/stylesheet/docbook-xsl/manpages/docbook.xsl manual.xml
	gzip -f -9  *.1
	cp -f *.1.gz ../pkg/usr/share/man/man1
	chmod 0644 ../pkg/usr/share/man/man1/*

clean:
	rm -f  *.gz
