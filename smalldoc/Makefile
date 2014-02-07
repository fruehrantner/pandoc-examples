DOCNAME = smalldoc
TEMPLATE = template

all:	html pdf

html:
	pandoc -f markdown -t html -s -o $(DOCNAME).html $(DOCNAME).md

pdf:
	pandoc -f markdown --latex-engine=lualatex --template=$(TEMPLATE).tex -o $(DOCNAME).pdf $(DOCNAME).md

clean:
	rm -f $(DOCNAME).html $(DOCNAME).pdf


