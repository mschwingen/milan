OPTIONS=--tabsize=8 --charset=latin --papersize=a4 --language=en

all:	pcibios.txt pcibios.dvi pcibios.html

pcibios.txt:	pcibios.sgml
	sgml2txt -f ${OPTIONS} pcibios

pcibios.dvi:	pcibios.sgml
	sgml2latex ${OPTIONS} pcibios

pcibios.sgml:	pcibios_.sgml
	sed -f sedfile <pcibios_.sgml >pcibios.sgml

pcibios.html:	pcibios.sgml
	sgml2html ${OPTIONS} --split=0 pcibios

clean:
	-rm *~ pcibios.sgml *.ps

distclean:	clean
	-rm *.dvi *.txt

.phony: all clean distclean









