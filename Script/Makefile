TEX := pdflatex
MAIN := main

.PHONY: all clean distclean

all: $(MAIN).pdf

$(MAIN).pdf: $(MAIN).tex
	$(TEX) -interaction=nonstopmode -halt-on-error $(MAIN).tex
	$(TEX) -interaction=nonstopmode -halt-on-error $(MAIN).tex

clean:
	rm -f $(MAIN).aux $(MAIN).log $(MAIN).out $(MAIN).toc

distclean: clean
	rm -f $(MAIN).pdf
