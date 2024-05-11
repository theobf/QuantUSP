bibfile=./refs.bib

all: memorandum.pdf

%.pdf: %.tex $(bibfile)
	pdflatex $<
	bibtex $*
	pdflatex $<
	pdflatex $<

.PHONY: clean
clean:
	rm -f *.log *.aux *.aux *.bbl *.blg *.out *.toc
