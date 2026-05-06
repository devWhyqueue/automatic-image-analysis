TEX := pdflatex
MAIN := main
TEX_SOURCES := $(MAIN).tex intro.tex
FIGURES := $(wildcard figures/*)

.PHONY: all clean distclean

all: $(MAIN).pdf

$(MAIN).pdf: $(TEX_SOURCES) $(FIGURES)
	$(TEX) -interaction=nonstopmode -halt-on-error $(MAIN).tex
	$(TEX) -interaction=nonstopmode -halt-on-error $(MAIN).tex

clean:
	rm -f $(MAIN).aux $(MAIN).log $(MAIN).out $(MAIN).toc

distclean: clean
	rm -f $(MAIN).pdf
