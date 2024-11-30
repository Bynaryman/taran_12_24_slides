TEX=pdflatex -shell-escape -interaction=nonstopmode -file-line-error
BIB=bibtex

STEM=main

TARGET=$(STEM).pdf
SRC = $(STEM).tex
AUX = $(STEM).aux

TARGET:
	$(TEX) $(SRC)
	$(BIB) $(STEM)
	$(TEX) $(SRC)
	$(TEX) $(SRC)


.PHONY: clean
clean:
	rm -f $(TARGET) $(AUX) *.bbl *.blg *.log *.out
